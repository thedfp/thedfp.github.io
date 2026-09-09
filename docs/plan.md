# The Plan

The plan has inputs and outputs. The plan inputs are:

- **Economic Information**: expected inflation, returns, etc.
- **Participants**: who, ages, and household information such as tax filing status
- **Accounts**: what accounts, where, what type, how much is in them in what positions and how much we are planning to add
- **Budget**: how much are planning to spend

The output for the plan engine should provide answers like: 

- Solving for the Monte Carlo success rate
    - For the total budget, the plan has a **92.7%** success rate.
    - For the required budget, the plan has a **99.9%** success rate.
- Solving for the maximum spending allowed
    - At a **90%** success rate, the **maximum sustainable budget is $204,881/yr**. On average, that is **$17,969/yr more** than your total annual budget. 

There are also some assumptions:

- Any single stock positions, such as ESPP or RSU accounts, have been sold and moved to broad-based ETFs or mutual funds. 
- Contributions to retirement cease when you retire
- Capital gains should always be long term. Always hold everything at least a year in taxable accounts.
- Monte Carlo results should be greater than 90% for a plan to be viable
- Bond positions should be in tax-deferred, equities in Roth and taxable accounts

## Economic Information

- **Inflation**: Used for calculating nominal values for non-healthcare costs
- **Healthcare Inflation**: Used for calculating nominal values for healthcare costs
- **Cost-of-Living Adjustment (COLA)**: Used for Medicare's adjustments for inflation
- **Tax Rates**
    - **Ordinary Income Tax**
    - **State Income Tax**
    - **Long Term Capital Gains Tax**
    - **Net Investment Income Tax**
    - **IRMAA Surcharges**

Some of these items will be able to be modeled for a plan. Some are baseline economic data that is what it is.

## Participants

Let's start with the people. Who's involved and what are some basic household facts. There's either one or two people.

- Participant(s)
    - Name
    - Date of Birth
    - Retirement Date
    - Life Expectancy
- Dependent(s)
    - Name
    - Date of Birth
    - Expected End of Dependency
- Household
    - Tax Filing Status (Single, Married Filing Jointly)
    - Where - City, State, Zip (Used for ACA subsidy calculations and state income tax impacts)

## Budget

Budgets should be annual and should be thoughtfully created. Remember, there are some expenses that may change dramatically when you cross certain age milestones - medicare being the biggest. You may go from paying full freight ACA marketplace health insurance for 3 or 4 people (~30-40k per year in Texas) to paying for medicare for 2 (~10k). You may also plan on traveling like mad people for the first 5-7 years and then dialing it back expecting possible grandchildren to be the focus. Don't just slap a number down and throw some inflation numbers at it. Put some thought into it.

One other piece of advice: round up. It's always better to have money allocated and not need it than to need it and not have it in the budget.

For every year from retirement until life expectancy of last participant:

- Year
- Total - Required + Discretionary
- Required - Base Living Expenses + Healthcare
- Healthcare Premiums - Just the premiums - we need these for modeling ACA subsidies, use the ACA benchmark premiums with no subsidy
- Healthcare Out of Pocket - We also want these because healthcare inflation is a different rate than regular inflation (higher, unfortunately)

## Financials

Where you are today and how much you are contributing to your retirement.

### Accounts

Accounts are where the money actually lives. The model needs enough detail per account to answer three questions: what is it worth, what does it cost in taxes to get money out of it, and when is that money legally available.

Most of that is not something you enter. The tax behavior falls out of the account type, which the model looks up from [Account Types](#account-types) rather than asking you to fill it in and get it wrong. That leaves a much shorter list of things that are actually yours to enter.

For each account:

- Account Name
- Account Type
- Owner (participant 1, participant 2, joint)
- Annual Contribution Amount
- Employer Match (employer plans only)
- Retired From This Employer (401k and 403b only)
- Position(s)

Owner matters more than it looks. Every age threshold in the budget section applies to a person, not a household. In a two participant plan, the same account type can be penalty-free for one spouse and locked to the other for years.

Retired From This Employer is the one piece the type cannot tell you. The rule of 55 only applies to the plan at the employer you actually separated from in or after the year you turn 55. Two identical 401ks, same owner, same age, and only one of them is available without a penalty.

For each position:

- Symbol
- Asset Class (equities, bonds, TIPS, cash)
- Bucket (cash, stable, growth)
- Shares
- Current Price
- Dividend Yield
- Dividend Treatment (qualified, non-qualified)
- Expense Ratio
- Lot(s)

Asset class is what connects a position to the expected returns in your plan. Bucket is the logical assignment from the three bucket system, and it is what tells the model which positions it is allowed to sell in a down year.

Dividends need their own treatment because they arrive whether you want them or not. Qualified dividends are taxed at capital gains rates and stack into the same 0% bracket you are trying to fill with sales, so they can quietly push a tax-free withdrawal plan into the 15% bracket.

For each lot:

- Quantity
- Acquisition Date
- Cost Basis

Lots only matter in taxable accounts. In a 401k or traditional IRA, everything that comes out is ordinary income no matter what you paid for it, so there is nothing worth tracking. In a brokerage account the acquisition date decides whether a sale is long-term or short-term, and the cost basis decides how much of the sale is taxable at all.

You do not tell the model which lots to sell. That is the whole reason to track them individually. Two lots of the same fund bought years apart produce completely different tax bills for the same dollar of spending, so the model picks the lots as part of solving the year.

A position's share count and market value are both derived from its lots rather than stored on their own. Balance is only entered directly for accounts that hold no positions, like checking. Storing the same number in two places is how the two drift apart.

### Annuities and Pensions

Pensions and annuities are income streams, not balances. You do not draw them down, you receive them, which makes them behave more like a paycheck than an account. Their job in the model is to reduce how much the portfolio has to produce.

For each income stream:

- Name
- Owner (participant 1, participant 2)
- Type (pension, immediate annuity, deferred annuity, QLAC)
- Start Age
- Annual Amount
- Real or Nominal (whether the amount above is in today's dollars)
- Cost of Living Adjustment (none, fixed percentage, tied to inflation)
- Tax Treatment (ordinary, partially taxable, tax-exempt)
- Modified Adjusted Gross Income Treatment
- Survivor Benefit (percentage that continues to a surviving spouse)
- Duration (life, joint life, period certain)
- Cost Basis (non-qualified annuities only)
- Lump Sum Option (pensions only)

The cost of living adjustment is the field that quietly decides whether the income is worth what it looks like. Most private pensions and most fixed annuities have no COLA at all. A $36,000 a year pension with no adjustment still pays $36,000 in thirty years, but at 3% inflation that is worth about $14,800 in today's dollars. It is the same number on the check and 41% of the groceries. This is exactly the real versus nominal problem, and it is why the model needs to know which kind of dollars the amount is stated in.

Taxation depends on where the money came from. A pension funded with pretax dollars and a qualified annuity held inside an IRA are both fully ordinary income. A non-qualified annuity bought with money you already paid tax on is different: each payment is part return of your own principal, which is not taxed, and part earnings, which are. That split is the exclusion ratio, and it needs the cost basis to calculate. Once the basis is used up, the payments become fully taxable.

Survivor benefit matters more in a two participant plan than most people expect. A pension that pays $60,000 while both spouses are alive and nothing afterward creates a cliff on the first death, at the same moment the household drops to single filer tax brackets. A 50% survivor election lowers the payment now to avoid that cliff later, and the model should be able to show you both versions.

Guaranteed income also changes how the guardrails behave. Guardrails are calculated on the portfolio withdrawal rate, so income that arrives regardless of the market means the portfolio has less work to do and a market drop cuts a smaller number. If pensions and Social Security together cover your required budget, the floor aware rule is satisfied no matter what the market does, which is the most robust position a plan can be in.

### Social Security

Social Security is guaranteed income like a pension, but it gets its own section because two parts of it are model machinery rather than data entry: when you claim it, and how much of it is taxable.

For each participant:

- Primary Insurance Amount (the monthly benefit at full retirement age)
- Full Retirement Age
- Claiming Age
- Earnings History (only if the model computes the PIA instead of taking it from your statement)
- Spousal Benefit Eligibility
- Survivor Benefit Assumption

The Primary Insurance Amount is the anchor. It is what you would receive at full retirement age, it comes straight off your Social Security statement, and every other number is a percentage of it. Claiming early permanently reduces it and claiming late permanently increases it. For a full retirement age of 67:

| Claiming Age | Benefit |
| ------------ | ------- |
| 62           | 70.0%   |
| 63           | 75.0%   |
| 64           | 80.0%   |
| 65           | 86.7%   |
| 66           | 93.3%   |
| 67           | 100.0%  |
| 68           | 108.0%  |
| 69           | 116.0%  |
| 70           | 124.0%  |

Claiming age is not really an input. It is one of the most valuable decisions in the whole plan, and it belongs with the other solved decisions. Delaying means spending down the portfolio to bridge the gap, which looks bad in isolation, but what you buy with it is a larger stream of income that is adjusted for inflation every year and lasts as long as you do. Unlike almost every private pension, Social Security has a real COLA, so the erosion problem does not apply to it.

Taxation works differently than everything else on this page and catches people off guard. You do not simply add the benefit to your income. Instead you calculate provisional income, which is your other income plus tax-exempt interest plus half of your Social Security benefit, and compare it to a set of thresholds.

- Below the first threshold, none of the benefit is taxable.
- Between the two, up to 50% becomes taxable.
- Above the second, up to 85% becomes taxable.

No more than 85% of the benefit is ever taxable, so it always gets better treatment than an IRA withdrawal.

!!! note "These thresholds do not move"
    The provisional income thresholds are fixed in statute and have never been indexed for inflation. Every year of raises and every cost of living adjustment pushes more retirees over lines that were drawn decades ago. They are reference data the model has to maintain, and they change only when Congress changes them.

This creates what is often called the tax torpedo. Inside the phase-in range, one more dollar pulled from a traditional IRA does not just get taxed itself, it also drags up to another 85 cents of Social Security into taxable income. A retiree who thinks they are in the 22% bracket is really paying about 41% on that dollar, and someone in the 12% bracket is paying about 22%. This is the clearest example on this page of why the marginal rate that matters is the one on your next dollar, not the one on your bracket, and it is a large part of why withdrawal sourcing has to be solved rather than guessed.

Married households need the survivor case modeled explicitly. When the first spouse dies, the household keeps the larger of the two benefits and loses the smaller one entirely. That happens in the same year the survivor drops to single filer brackets, so income falls and the tax rate on what remains goes up. Delaying the higher earner's claim to 70 is often less about that person and more about locking in the largest possible benefit for whoever lives longer.

## Plan Calculation Engine

The plan calculation engine should answer several questions for the participants.

- **Plan Viability**: Will you always have enough money based on your estimated budget? At what confidence is that calculated?
- **Maximum Spending Thresholds**: How much can I spend? Can I reasonably spend more than I have budgeted?
- **Immediate Retirement**: If I retired tomorrow, what would the maximum spending look like over the plan lifetime?

### Decisions and Constraints

The plan also requires optimizations for the following aspects:

- Withdrawal Sourcing (which accounts to draw from, and in what order)
    - In taxable accounts, lot ordering is also a solvable constraint
- Social Security Claiming Age (between 62 and 70, for each participant)
    - This should take into account total social security value and spousal claims
- Roth Conversion Optionality (if so, how much to convert, when and what tax impact would it have)
- How to minimize lifetime tax payments across all tax types

### Stress Testing

The plan should be stress tested against all of the following scenarios:

- Monte Carlo - 10,000 runs
- Historicals - Use historical data from recent market crashes
    - Global Financial Crisis (GFC) 2007-2009
    - COVID-19 Pandemic Crash 2020
    - 2022 Inflation & Rate Hike Bear Market
    - 2018 Trade & Rate Scare

## Reports

Here's a list of the output measures for the plan engine with example values. 

| Measure                                                           |            Value |
| --------------------------------------------------------------    | ---------------: |
| Current Portfolio Value                                           |       $2,000,000 |
| Current Equity ratio                                              |              95% |
| Current Bond ratio                                                |               2% |
| Current Cash ratio                                                |               3% |
| Retirement Portfolio Value                                        |       $4,000,000 |
| Retirement Equity ratio                                           |              55% |
| Retirement Bond ratio                                             |              35% |
| Retirement Cash ratio                                             |              10% |
| Required spending                                                 |     $100,000 /yr |
| Discretionary spending — budgeted                                 |      $50,000 /yr |
| Total budgeted                                                    |     $150,000 /yr |
| Success at the required budgeted spend                            |           100.0% |
| Success at the total budgeted spend                               |            92.7% |
| Maximum sustainable spend (10,000 trials, historical)             |     $204,881 /yr |
| Maximum sustainable spend — historical, 2,000-trial sweep         |     $200,123 /yr |
| Maximum sustainable spend — forward-looking, 2,000-trial sweep    |     $174,223 /yr |
| Median terminal estate at the budgeted spend, before tax          |      $11,280,263 |
| Median terminal estate, after tax to heirs                        |      $11,099,892 |
| 10th-percentile terminal estate, before tax                       |         $690,424 |

| Measure                                                           |            Value |
| --------------------------------------------------------------    | ---------------  |
| Participant 1 - Social Security Claim Age                         |               70 |
| Participant 2 - Social Security Claim Age                         |               70 |


- What do I need to do this year?
- What do I need to do over the next 3 years?
- What does my year by year financial projection look like?
    - year, ages, spending, returns, portfolio