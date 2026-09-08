# The Digital Financial Planner

When building a financial plan, there are many of large questions we want answered.  

* Am I saving enough to reach my goals?
* Based on what I have and how much I am saving, if I retired on a particular date, what would be my maximum annual spending budget?
* Based on desired budget projections, how much do I need invested? 
* Do I have enough to leave a desired terminal estate for my beneficieries? 

Things we do not know

* What are taxes going to be like in the future?
* How will the markets react? 
* What will inflation be like, especially around healthcare?
* Will the subsidies around healthcare be around in 5 or 10 years?

# Knowledge and Concepts

The entire concept around retirement is simple: Can I save up enough money so that in the future, that money can generate returns that are enough to retire on? Many people read that as "living off the returns only" but that's not what it says. While the returns only retirement plan is a viable one, most people don't have enough money to allow it to sit untouched and just live off of it.

For a very long time, there was a concept called the 4% rule which was created by William Bengen and published in 1994. Take your portfolio every year, withdraw 4% of it, and that is your spending budget for the year including taxes. The 4% rule is considered outdated and even Bengen himself has updated his guidance. It's also very rigid and doesn't truly encapsulate the strategies that allow your spending rules to flex with the markets. 

Linear projections are also used as crude retirement tools. Take what you want to spend, adjust it for inflation through your life expectancy, and then take your portfolio, add expected returns, subtract the spending and boom, there's your plan. But we all know that's not the way markets work. They aren't flat. Inflation isn't flat, especially healthcare costs. While linear projections provide a simple foundation, they shouldn't be used in practice for planning your retirement. 

## Real and Nominal Dollars

Nominal dollars are the actual dollar amounts you see, earn, or spend at a given point in time—without adjusting for inflation. It is the unadjusted "face value" printed on paper currency or written on a paycheck.

Example: If you earned $50,000 in 2010 and earn $50,000 today, your income in nominal dollars is identical ($50,000).

Real dollars measure the actual quantity of goods and services that money can buy by adjusting nominal figures for inflation. Real dollars express value relative to a specific base year, removing the distorting effects of price changes over time.

Real dollars are used to denote purchasing power and are used extensively in your budget. You should model your projected spending as what things cost today and then let the inflation projections then create the nominal dollars representing your actual spend throughout your retirement. 

## Marginal Tax Rates

So many people don't understand marginal tax rates. They think that if you make more money and you move to the next tax bracket, that all of your income is suddenly taxed at that next level. Marginal tax rates apply across your income so that if you are lucky enough to move into the next bracket, only that income in the range for the next bracket is taxes at that higher level. Here's an example of someone making $120,000 a year (single). 

| Amount              | Rate  | Amount in Bracket | Tax Paid  |
| -----------         | ----- | ---               | ---       |
| $0 - $12,400        | 10%   | $12,400           | $1,240    |
| $12,401 – $50,400   | 12%   | $38,000           | $4,560    |
| $50,401 – $105,700  | 22%   | $55,300           | $12,166   |
| $105,701 – $201,775 | 24%   | $14,300           | $3,432    |

**Total Tax Paid:** $21,398 (not $28,800)


## Income vs AGI vs MAGI

Gross Income (Total Income): The starting point. This includes all income from all sources before any deductions or adjustments (W-2 wages, 1099 income, capital gains, dividends, traditional IRA distributions, rental income, business profits, taxable Social Security, etc.).

Adjusted Gross Income (AGI): Found on Line 11 of Form 1040. This is your Gross Income minus specific "Above-the-Line" deductions (such as pre-tax HSA contributions, traditional IRA deductions, self-employed health insurance premiums, 401(k)/SEP-IRA contributions for self-employed individuals, or student loan interest deductions).

Modified Adjusted Gross Income (MAGI): MAGI takes your AGI and adds back certain tax-exempt or specialized items that the government doesn't want you using to artificial lower your income eligibility for subsidies or lower tax rates.

Crucial Detail: There is no single definition of MAGI. The IRS defines MAGI differently depending on the specific tax credit, program, or penalty being calculated.


## Guardrails

## Three Bucket System

* Cash - Covers immediate living expenses for 3-5 years. This bucket is actually two - checking and "savings". Your checking should be liquid with 3-6 months of spending in it. Your savings should have the rest and should be in something that is inflation adjusted, like SCHP. 

* Stable - Provides income and capital preservation for the medium term (typically years 3 to 10). Treasury bonds, high-grade corporate bonds, multi-asset income funds, or CD ladders. Moderate growth with lower volatility than stocks, acting as a reservoir to replenish Bucket 1 when cash runs low.

* Growth - Long-term capital growth for the remaining horizon (years 10+). Broad-market equity index funds, dividend-growth stocks, or real estate investment trusts (REITs). The goal is in the name - growth. Capital appreciation. Since this money won't be needed for a decade or more, it has time to recover from short-term market crashes.

Remember the buckets are logical, not accounts. Your cash might be in a checking account and your "savings" might be in your brokerage account. Your stable bucket could be spread across your 401k and traditional IRA. Same with growth. 

# The Model

## Participants

Modeling is built around 1 or 2 participants.  
Dependents are included for tax and ACA subsidy calculation purposes.  

- Tax Filing Status (Single, Married Filing Jointly)  

## Budget 

Budgets are flexibly modeled around three industry standard phases of retirement  

- Go-Go: up to 70 years old, these years you are hopefully unrescrited from any physical limitaions such as travel or other adventures
- Slow-Go: 70 to 80 years old, these years are punctuated by a marked slow down in travel or activities  
- No-Go: 80 until life expectancy, these years are marked with little travel and advanture, usually focused on family and health  

Budgets also follow some key age thresholds which will influence your contributions and spending  

- 50 - Participants eligible for catch-up contributions
- 60 to 63 - Participants eligible for additional catch-up contributions
- 55 - The rule of 55 gives access without penalty to 401(k) funds if the participant retires from the company holding the 401(k) after or in the year the participant turns 55. You can also start Health Savings Account (HSA) catch-up contributions at age 55.
- 59.5 - Participant has full access to all retirement funds without penalty  
- 62 - You become eligible to collect early Social Security retirement benefits, though doing so permanently reduces your monthly payout
- 65 - Participant is eligible for Medicare
- 67 - Full Retirement Age (FRA) to collect 100% of your calculated Social Security benefit. 
- 70 - Delaying Social Security stops increasing your monthly benefit, making it the optimal age to start claiming if you waited.
- 75 - Required Minimum Distributions (RMDs) begin for participants born in 1960 or later
    - 73 for those born between 1951 and 1959

A retirement budget isn't a fixed point, but rather an acceptable range of values. These range of values can also change from year to year, depending on the type of spending it is.

- Total - a yearly projection in real dollars of what you want to spend including everything you want
- Required - this is the bare minimum amount needed to "survive". This will be different for everyone as some may choose to include spending in their required budget that others would look at as purely discretionary. 
    - Healthcare - Healthcare includes two components: insurance premiums and expected out of pocket costs

Other one-time or time-boxed expenses may inflence your budget projections. Again, some of these would be considered discretionary and some may be required, depending on your wants and needs. 

- Dependent Expenses - college, cars, healthcare, financial support
- Events - Weddings, parties, moving to Hawaii
- Fixed Payments - Car, Boat, House

Your spending is the money going out the door. This does not include taxes. Your taxes are the costs associated with generating the "income" needed to supply the cash for the spending. These include: 

- Ordinary Income Taxes
- State Income Taxes
- Capital Gains Taxes
- Net Investment Income Tax (NIIT)
- IRMAA surcharges

Additionally, we want a flexible budget because we will need to flex with the portfolio. Especially during years when the market is down, we want to leave our growth positions such as our equity positions alone while they are in a depressed state. Having to sell equities during down years at a low value does significant damage to the long term viability of the plan. Therefore we want to be able to flex with the market. If the market is down, our spending should follow suit. If the market comes back up, so can our spending. Our spending guardrails in combination with our bucket strategy will allow our equity growth positions to remain untouched at their most vulnerable. 

## Financials

Where you are today and how much you are contributing to your retirement

### Accounts

For each account  

* Account Type (checking, brokerage, 401k, Roth 401k, Traditional IRA, Roth IRA, HSA, 403b, etc)
* Contribution Tax Treatment (pretax, posttax)
* Withdrawal Tax Treatment (ordinary, tax-exempt, capital gains)
* Modified Adjusted Gross Income Treatment
* Balance
* Annual Contribution Amount
* Position(s)
    * Asset
    * Value
    * Lot(s)

### Annuities and Pensions

### Social Security

## Plan

### Required Economic Values

- Expected Inflation
- Expected Returns for Asset Classes (equities, bonds, etc)
- Marginal Tax Rates (brackets, income, percent)
- Capital Gains Tax Rates (year_through, percent, tax filing status, income)
- IRMAA 
- Social Security Calculations

### Calculation Strategies 

- Linear
- Guardrails

### Stress Testing

- Monte Carlo
- Historicals

## Reports

* What do I need to do this year?
* What do I need to do over the next 3 years?
* What does my year by year financial projection look like?