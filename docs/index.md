# The Digital Financial Planner

When building a financial plan, there are many large questions we want answered.

- Am I saving enough to reach my goals?
- Based on what I have and how much I am saving, if I retired on a particular date, what would be my maximum annual spending budget?
- Based on desired budget projections, how much do I need invested?
- Do I have enough to leave a desired terminal estate for my beneficiaries?

How much you have is one aspect of your retirement planning. Another big one is where you have it. There are a ton of tax implications and other opportunities to those who understand the full range of account options. For example, if you plan on retiring before the age of 59.5, which is when tax-advantaged accounts like IRAs and 401k are available without a penalty, you better have some retirement funds available to you in a brokerage account.

There are also a ton of things we do not know.

- What are taxes going to be like in the future?
- How will the markets react?
- What will inflation be like, especially around healthcare?
- Will the subsidies around healthcare be around in 5 or 10 years?

For all of these, that's where we want to test the plan. We want to take a bunch of different values, some good, some bad and throw them at the plan to see what happens and how everything works out. Don't expect a huge market meltdown? So did the people that retired in 2000. And 2006. And 2019. The point of the model is to test all of these "worst case" scenarios and see what happens. It seems like we live in a world full of one in a lifetime events every year or so. Let's plan on it to happen and give yourself some peace of mind that you won't be welcoming someone to Walmart in your golden years.

## Knowledge and Concepts

The entire concept around retirement is simple: Can I save up enough money so that in the future, that money can generate returns that are enough to retire on? Many people read that as "living off the returns only" but that's not what it says. While the returns only retirement plan is a viable one, most people don't have enough money to allow it to sit untouched and just live off of it.

For a very long time, there was a concept called the 4% rule which was created by William Bengen and published in 1994. Take your portfolio every year, withdraw 4% of it, and that is your spending budget for the year including taxes. The 4% rule is considered outdated and even Bengen himself has updated his guidance. It's also very rigid and doesn't truly encapsulate the strategies that allow your spending rules to flex with the markets.

Linear projections are also used as crude retirement tools. Take what you want to spend, adjust it for inflation through your life expectancy, and then take your portfolio, add expected returns, subtract the spending and boom, there's your plan. But we all know that's not the way markets work. They aren't flat. Inflation isn't flat, especially healthcare costs. While linear projections provide a simple foundation, they shouldn't be used in practice for planning your retirement.

Let's walk through some core concepts that are integral to understanding retirement.

### Real and Nominal Dollars

**Nominal dollars** are the actual dollar amounts you see, earn, or spend at a given point in time, without adjusting for inflation. It is the unadjusted "face value" printed on paper currency or written on a paycheck. If you earned $50,000 in 2010 and earn $50,000 today, your income in nominal dollars is identical.

**Real dollars** measure the actual quantity of goods and services that money can buy by adjusting nominal figures for inflation. Real dollars express value relative to a specific base year, removing the distorting effects of price changes over time.

Real dollars are used to denote purchasing power in today's dollars and are used extensively in your budget. You should model your projected spending as what things cost today and then let the inflation projections then create the nominal dollars representing your actual spend throughout your retirement.

### Income vs AGI vs MAGI

**Gross Income**: The starting point. Total income. This includes all income from all sources before any deductions or adjustments (W-2 wages, 1099 income, capital gains, dividends, traditional IRA distributions, rental income, business profits, taxable Social Security, etc.).

**Adjusted Gross Income (AGI)**: Found on Line 11 of Form 1040. This is your Gross Income minus specific "Above-the-Line" deductions (such as pre-tax HSA contributions, traditional IRA deductions, self-employed health insurance premiums, 401(k)/SEP-IRA contributions for self-employed individuals, or student loan interest deductions).

**Modified Adjusted Gross Income (MAGI)**: MAGI takes your AGI and adds back certain tax-exempt or specialized items that the government doesn't want you using to artificially lower your income eligibility for subsidies or lower tax rates.

!!! note "Crucial Detail"
    There is no single definition of MAGI. The IRS defines MAGI differently depending on the specific tax credit, program, or penalty being calculated.

### Marginal Tax Rates

So many people don't understand marginal tax rates. They think that if you make more money and you move to the next tax bracket, that all of your income is suddenly taxed at that next level. Marginal tax rates apply across your income so that if you are lucky enough to move into the next bracket, only that income in the range for the next bracket is taxed at that higher level. Here's a very simple example of someone making $120,000 a year (single). This obviously does not take into account the standard or other deductions.

| Amount              | Rate      | Amount in Bracket |    Tax Paid |
| ------------------- | --------- | ----------------: | ----------: |
| $0 – $12,400        | 10%       |           $12,400 |      $1,240 |
| $12,401 – $50,400   | 12%       |           $38,000 |      $4,560 |
| $50,401 – $105,700  | 22%       |           $55,300 |     $12,166 |
| $105,701 – $201,775 | 24%       |           $14,300 |      $3,432 |
| **Totals/Avg**      | **17.8%** |      **$120,000** | **$21,398** |

This person's effective tax rate is 17.8%, not 24% even though they make enough to be in that "bracket".

### Account Types

How much you have matters. Where you keep it matters just as much. Every account type carries its own rules about how money goes in, how it comes out, and when you are allowed to touch it without a penalty.

| Account Type       | Contributions | Withdrawals            | MAGI | Early Withdrawal                        | RMDs |
| ------------------ | ------------- | ---------------------- | ---- | --------------------------------------- | ---- |
| Checking / Savings | Posttax       | Not taxed              | No   | None                                    | No   |
| Brokerage          | Posttax       | Capital gains          | Yes  | None                                    | No   |
| 401k / 403b        | Pretax        | Ordinary               | Yes  | 59.5, or 55 on separation               | Yes  |
| Roth 401k / 403b   | Posttax       | Tax-exempt             | No   | 59.5, or 55 on separation               | No   |
| 457(b)             | Pretax        | Ordinary               | Yes  | Any age on separation                   | Yes  |
| Traditional IRA    | Pretax        | Ordinary               | Yes  | 59.5                                    | Yes  |
| SEP / SIMPLE IRA   | Pretax        | Ordinary               | Yes  | 59.5                                    | Yes  |
| Roth IRA           | Posttax       | Tax-exempt             | No   | Contributions anytime, earnings at 59.5 | No   |
| HSA                | Pretax        | Tax-exempt for medical | No   | Medical anytime, otherwise 65           | No   |

A few of these carry conditions that a single row cannot capture.

- **HSA**: Withdrawals are tax-exempt for qualified medical expenses at any age. Non-qualified withdrawals before 65 are ordinary income plus a 20% penalty, and after 65 they are ordinary income with no penalty.
- **Traditional IRA**: Contributions are only deductible if your income is below the phase-out, and the phase-out depends on whether you or your spouse are covered by a workplace plan.
- **Roth IRA**: Contributions can come out at any time tax-free and penalty-free. Earnings need both age 59.5 and the five year clock.
- **SIMPLE IRA**: The early withdrawal penalty is 25% rather than 10% during your first two years in the plan.

This is why your retirement date drives which accounts you need. Retire at 55 and a brokerage account does the heavy lifting for years before your 401k opens up without a penalty. Retire at 67 and that gap never exists.

### Required Minimum Distributions

**Required Minimum Distributions (RMDs)** are mandatory withdrawals that the IRS requires you to take each year from tax-deferred retirement accounts once you reach a certain age.

Because traditional retirement accounts allow your contributions and investment earnings to grow tax-deferred for decades, the government uses RMDs to ensure it eventually collects income tax on those funds.

- **Starting age**: 73 for participants born between 1951 and 1959, and 75 for those born in 1960 or later.
- **Accounts subject to RMDs**: Traditional, SEP and SIMPLE IRAs, along with 401(k), 403(b) and 457(b) plans.
- **Accounts exempt**: Roth IRAs are exempt for the original owner, and Roth 401(k)s became exempt during your lifetime starting in 2024.
- **Calculation method**: Your account balance as of December 31 of the previous year, divided by a life expectancy factor from the IRS Uniform Lifetime Table.
- **Deadlines**: Your first RMD is due by April 1 of the year after you reach your starting age. Every one after that is due by December 31.
- **Penalty**: RMDs are taxed as ordinary income. Missing one draws a 25% excise tax on the amount you failed to withdraw, reduced to 10% if you correct it promptly.

Two strategies come up over and over for managing them.

- **Roth conversions**: Converting pretax funds to a Roth before your starting age reduces the tax-deferred balance, which shrinks every future required distribution.
- **Qualified charitable distributions**: From age 70.5 you can send money directly from a Traditional IRA to a qualified charity, up to an annually indexed limit. It satisfies the RMD and stays out of your taxable income entirely.

### Sequence of Returns Risk

**Sequence of returns risk** (or sequence risk) is the danger that the timing of market downturns will negatively impact the total value of your portfolio, specifically when you are withdrawing money in early retirement.

Even if two retirees experience the exact same average market return over a 20-year period, the person who experiences market losses in the first few years of retirement is at a much higher risk of running out of money than someone who sees market gains early on.

#### Why It Matters

During your working years, a market drop works in your favor because you are continuously buying shares at a discount (dollar-cost averaging). Once you retire and start withdrawing income, market drops work in reverse and you end up selling low.

1. **Market drops**: Your portfolio value falls.
2. **You withdraw funds**: To meet living expenses, you must liquidate and sell more shares than usual while prices are low.
3. **Loss is permanent**: Those sold shares are gone forever. When the market eventually rebounds, you have fewer shares left in your account to participate in the recovery.

#### A Tale of Two Retirees

Imagine two retirees, Retiree A and Retiree B, who both start with $1,000,000 and withdraw $50,000 per year. They get the exact same three market returns of +20%, +5%, and -20%. The only difference is the order they arrive in.

| Year   | A's Return | A's Balance | B's Return | B's Balance |
| ------ | ---------- | ----------- | ---------- | ----------- |
| Year 1 | +20%       | $1,150,000  | -20%       | $750,000    |
| Year 2 | +5%        | $1,157,500  | +5%        | $737,500    |
| Year 3 | -20%       | $876,000    | +20%       | $835,000    |

Same three returns, same withdrawals, same average — but Retiree B ends Year 3 with $41,000 less, simply because the bad year happened at the very beginning.

#### Common Strategies to Mitigate Sequence Risk

- **Dynamic withdrawal rules**: Use strategies like the Guyton-Klinger Guardrails to trim your annual withdrawals slightly during market dips, preserving portfolio principal.
- **Three bucket system**: Keep 3 years' worth of living expenses in cash and short-term bonds. During a stock market crash, pull income from this buffer instead of selling equities at a discount.
- **Flexibility in spending**: Differentiate between core expenses (housing, groceries) and discretionary spending (travel, dining) so you can temporarily cut back during down markets.

### Guardrails

The **Guyton-Klinger (GK) Guardrails** approach is a dynamic strategy for pulling income from your retirement portfolio.

Instead of following a rigid rule, like taking out a set 4% every single year adjusted for inflation, the guardrails method acts like lane markers on a highway. It allows you to start with a higher initial spending rate, often around 5%, but requires you to make small adjustments up or down depending on market performance.

#### How It Works

1. **Set your target withdrawal rate**: You choose an initial percentage to take out in Year 1, for example 5% of a $1,000,000 portfolio, or $50,000.
2. **Define the upper guardrail**: This is the pay raise. If strong market gains drive your portfolio up, causing your withdrawal rate to drop 20% below your target, down to 4%, you give yourself a 10% spending bump.
3. **Define the lower guardrail**: This is the pay cut. If a market crash drags your portfolio down, causing your withdrawal rate to jump 20% above your target, up to 6%, you trim your withdrawals by 10% to protect your principal.
4. **Inflation adjustment**: In normal years, you increase your spending to match inflation, but you skip this raise after a negative market year.
5. **Floor aware**: If the lower guardrail ever cuts below your required budget, then your plan is not a valid plan.

#### A Simple Example

Starting with a $1,000,000 portfolio and a target rate of 5%, or a $50,000 annual draw.

- **Upper guardrail**: Triggered if the portfolio grows to $1.25M. Increase the payout to $55,000.
- **Lower guardrail**: Triggered if the portfolio drops to $833,000. Trim the payout down to $45,000.

#### Why People Use It

- **Higher starting income**: You get to enjoy more of your money during the active, early years of retirement compared to static traditional rules.
- **Safety against running out**: Temporary 10% spending cuts during bad market dips prevent you from over-draining your nest egg when stocks are down, avoiding sequence of returns risk.
- **No guesswork**: You know in advance exactly at what portfolio numbers you get a raise or need to trim back.

### Three Bucket System

The bucket horizons are not arbitrary. They come from how long the market has historically taken to climb back after a drop.

- **Minor pullbacks (5% drop)**: Usually recover in 1 month or less.
- **Corrections (10% to 20% drop)**: Average about 3 to 8 months to recover.
- **Bear markets (20% to 30% drop)**: Average about 1 to 2 years to recover, though non-recession drops (like 2020) can bounce back in just a few months.
- **Severe crashes (30% or more drop)**: Can take 3 to 7+ years to reach previous highs, especially if tied to a deep economic recession or financial crisis.

A severe crash can take 3 to 7+ years to recover, so the buckets are sized to keep you from ever having to sell growth positions inside that window.

- **Cash**: Covers immediate living expenses for the next 3 years. This bucket is actually two — checking and "savings". Your checking should be liquid with 3–6 months of spending in it. Your savings should have the rest and should be in something that is inflation adjusted, like SCHP.
- **Stable**: Provides income and capital preservation for the medium term, typically years 3 to 10. Treasury bonds, high-grade corporate bonds, multi-asset income funds, or CD ladders. Moderate growth with lower volatility than stocks, acting as a reservoir to replenish the cash bucket when it runs low.
- **Growth**: Long-term capital growth for the remaining horizon, years 10 and beyond. Broad-market equity index funds, dividend-growth stocks, or real estate investment trusts (REITs). The goal is in the name — growth. Capital appreciation. Since this money won't be needed for a decade or more, it has time to recover from short-term market crashes.

The size of these buckets should match **your** risk tolerances.

Remember the buckets are logical, not account-based. Your cash might be in a checking account and your "savings" might be in your brokerage account. Your stable bucket could be spread across your 401k and traditional IRA. Same with growth.

Additionally, these buckets can also be much more aggressive. There are some opinions that only 2 buckets are needed: Cash bucket with 6 months in checking and 18 months in [SCHP](https://www.schwabassetmanagement.com/products/schp) and a Growth bucket for the rest in [VTI](https://investor.vanguard.com/investment-products/etfs/profile/vti). And if additional funds are needed for a downturn, only sell VTI in small chunks (think 2 months of spend) if the recovery takes longer than 2 years.

### Building a Retirement Budget

Budgets are flexibly modeled around three industry standard phases of retirement.

- **Go-Go**: Up to 70 years old, these years you are hopefully unrestricted from any physical limitations such as travel or other adventures.
- **Slow-Go**: 70 to 80 years old, these years are punctuated by a marked slow down in travel or activities.
- **No-Go**: 80 until life expectancy, these years are marked with little travel and adventure, usually focused on family and health.

Budgets also follow some key age thresholds which will influence your contributions and spending.

- **50**: Participants eligible for catch-up contributions.
- **55**: The rule of 55 gives access without penalty to 401(k) funds if the participant retires from the company holding the 401(k) after or in the year the participant turns 55. You can also start Health Savings Account (HSA) catch-up contributions at age 55.
- **59.5**: Participant has full access to all retirement funds without penalty.
- **60–63**: Participants eligible for additional catch-up contributions.
- **62**: You become eligible to collect early Social Security retirement benefits, though doing so permanently reduces your monthly payout.
- **65**: Participant is eligible for Medicare.
- **67**: Full Retirement Age (FRA) to collect 100% of your calculated Social Security benefit.
- **70**: Delaying Social Security stops increasing your monthly benefit, making it the optimal age to start claiming if you waited.
- **75**: Required Minimum Distributions (RMDs) begin for participants born in 1960 or later, or 73 for those born between 1951 and 1959.

A retirement budget isn't a fixed point, but rather an acceptable range of values. These ranges of values can also change from year to year, depending on the type of spending it is.

- **Total**: A yearly projection in real dollars of what you want to spend including everything you want.
- **Required**: The bare minimum amount needed to "survive". This will be different for everyone as some may choose to include spending in their required budget that others would look at as purely discretionary. Healthcare includes two components: insurance premiums and expected out of pocket costs.

Other one-time or time-boxed expenses may influence your budget projections. Again, some of these would be considered discretionary and some may be required, depending on your wants and needs.

- **Dependent Expenses**: College, cars, healthcare, financial support.
- **Events**: Weddings, parties, moving to Hawaii.
- **Fixed Payments**: Car, boat, house.

### Taxes

Your budget is the money going out the door. This does not include tax obligations generated when selling assets to fund your spending. Your taxes are the costs associated with generating the "income" needed to supply the cash for the spending. These include:

| Tax Type                         | Structure         | Description & Key Mechanism |
| -------------------------------- | ----------------- | --- |
| Ordinary Income Taxes            | Marginal          | Federal income tax brackets range from 10% to 37%. Tax rates apply only to the portion of income within each specific bracket, not to your entire income. |
| State Income Taxes               | Marginal (mostly) | Most states with an income tax utilize progressive marginal brackets. A few states use a single flat rate, and specific state exemptions/credits can occasionally introduce localized cliff effects. |
| Capital Gains Taxes              | Marginal          | Long-term capital gains rates (0%, 15%, 20%) are structured marginally based on taxable income thresholds. Short-term capital gains are taxed as ordinary income (also marginal). |
| Net Investment Income Tax (NIIT) | Phase-in / Hybrid | A 3.8% tax applied to the *lesser* of net investment income or the amount of MAGI exceeding the threshold ($200,000 single / $250,000 MFJ). Because it applies only to the excess over the threshold, it prevents a hard cliff. |
| IRMAA Surcharges                 | Cliff             | Medicare Part B and Part D premium surcharges use strict income tiers based on MAGI from two years prior. Earning $1 over a tier threshold triggers the full surcharge rate across the entire year. |

Additionally, we want a flexible budget because we will need to flex with the portfolio. Especially during years when the market is down, we want to leave our growth positions such as our equity positions alone while they are in a depressed state. Having to sell equities during down years at a low value does significant damage to the long term viability of the plan. Therefore we want to be able to flex with the market. If the market is down, our spending should follow suit. If the market comes back up, so can our spending. Our spending guardrails in combination with our bucket strategy will allow our equity growth positions to remain untouched at their most vulnerable.

Part of the plan is to try not to pay taxes. The other part is that if you have to pay taxes, pay as little as possible. The other other part is to look for opportunities to pay less in taxes now if you are expecting to pay more in taxes later (Roth conversions).

## The Plan

The plan has inputs and outputs. The plan inputs are:

- **Economic Information**: expected inflation, returns, etc.
- **Participants**: who, ages, and household information such as tax filing status
- **Accounts**: what accounts, where, what type, how much is in them in what positions and how much we are planning to add
- **Budget**: how much are planning to spend

There are also some assumptions:

- Contributions to retirement cease when you retire
- Capital gains should always be long term. Always hold everything at least a year in taxable accounts.
- Monte Carlo results should be greater than 90% for a plan to be viable

### Economic Information

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

### Participants

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

### Budget

Budgets should be annual and should be thoughtfully created. Remember, there are some expenses that may change dramatically when you cross certain age milestones - medicare being the biggest. You may go from paying full freight ACA marketplace health insurance for 3 or 4 people (~30-40k per year in Texas) to paying for medicare for 2 (~10k). You may also plan on traveling like mad people for the first 5-7 years and then dialing it back expecting possible grandchildren to be the focus. Don't just slap a number down and throw some inflation numbers at it. Put some thought into it.

One other piece of advice: round up. It's always better to have money allocated and not need it than to need it and not have it in the budget.

For every year from retirement until life expectancy of last participant:

- Year
- Total - Required + Discretionary
- Required - Base Living Expenses + Healthcare
- Healthcare Premiums - Just the premiums (we need these for modeling ACA subsidies)
- Healthcare Out of Pocket - We also want these because healthcare inflation is a different rate than regular inflation (higher, unfortunately)

p.s. Don't buy the boat.

### Financials

Where you are today and how much you are contributing to your retirement.

#### Accounts

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

#### Annuities and Pensions

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

#### Social Security

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

### Plan Calculation Engine

The plan calculation engine should answer several questions for the participants.

- **Plan Viability**: Will you always have enough money based on your estimated budget? At what confidence is that calculated?
- **Maximum Spending Thresholds**: How much can I spend? Can I reasonably spend more than I have budgeted?
- **Immediate Retirement**: If I retired tomorrow, what would the maximum spending look like over the plan lifetime?

#### Decisions and Constraints

The plan also requires optimizations for the following aspects:

- Withdrawal Sourcing (which accounts to draw from, and in what order)
    - In taxable accounts, lot ordering is also a solvable constraint
- Social Security Claiming Age (between 62 and 70, for each participant)
    - This should take into account total social security value and spousal claims
- Roth Conversion Optionality (if so, how much to convert, when and what tax impact would it have)
- How to minimize lifetime tax payments across all tax types

#### Stress Testing

The plan should be stress tested against all of the following scenarios:

- Monte Carlo - 10,000 runs
- Historicals - Use historical data from recent market crashes
    - Global Financial Crisis (GFC) 2007-2009
    - COVID-19 Pandemic Crash 2020
    - 2022 Inflation & Rate Hike Bear Market
    - 2018 Trade & Rate Scare

### Reports

- What do I need to do this year?
- What do I need to do over the next 3 years?
- What does my year by year financial projection look like?
    - year, ages, spending, returns, portfolio