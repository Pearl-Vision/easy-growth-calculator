# Easy Growth Planner

**Compare. Plan. Grow.** A compound interest planner that runs in the browser. It needs no install and no build step.

**Live app:** https://pearl-vision.github.io/easy-growth-calculator/

## What it does

- Enter a starting amount, a regular contribution (monthly, quarterly, half-yearly or yearly), a yearly interest rate and how often interest compounds (daily, monthly, quarterly, half-yearly or yearly). Compounding starts on yearly.
- Every number box starts at 0, so you type your own figures. The page starts fresh each time it opens.
- Choose a period of 1 to 50 years, with quick buttons for 10, 20, 30 and 40 years.
- Add inflation, either one rate for every year or a different rate for each year, to see the final value in today's money.
- See the results in summary tiles, a stacked growth chart and a year-by-year table.

## Compare options

- **Option A** is your main details.
- **Options B and C** each have their own contribution, rate, compounding and inflation (the same as A, or their own rate).
- **Option D** is either **buying a house** with a loan or **investing in shares**:
  - House: first choose **home to live in (PPR)** or **investment property**. Then enter the price, deposit, buying costs, yearly costs, loan term, house value growth and a loan rate that is fixed or changes each year (the repayment is worked out again when the rate changes). The final value is your equity: the house value minus the loan still owed.
  - Investment property also takes the weekly rent (with a yearly increase) and selling costs. Rent received lowers the money you put in, and selling costs come off the house value. Tax is not included.
  - Shares: starting amount, contribution, expected return and compounding. For **rent vs buy**, add the rent you would pay if not buying (with a yearly increase); it counts as money spent and does not grow. **Use the same money as the house** invests what is left after rent, so both put in the same total.
  - Option D can use Option A's inflation or its own.
- When you compare, the top card shows the **winner** (the biggest final value). The comparison shows a summary table, a chart you can switch between lines, bars, shaded areas and the difference from Option A, and year-by-year balances. The main year-by-year table adds columns for each option.

## Goal finder

- Type a goal (in future money, or in today's money allowing for inflation). Using Option A's settings, it shows how much to add each time to reach the goal in your chosen years, with a button to use that amount, and how long it takes with what you add now.

## Currencies

- Pick from 9 currencies, or type any other currency. The page guesses a starting currency from the device's time zone or region. It reads these from the device and does not send them anywhere. Your last currency choice is remembered in your own browser only.
- You type your own interest rates. Check current rates with your bank or a comparison website.

## Privacy

- Visits are counted anonymously with [GoatCounter](https://www.goatcounter.com/): no cookies and no personal data. It records only things like the page visited, the country, the type of device and where the visit came from.
- The amounts, rates and other numbers you type never leave your browser.
- Opening `index.html` from your own computer is not counted.
- The **Feedback / Contact** link opens a separate Google Form. Only what you choose to type there is sent (your email is optional), and Google stores it. The form is not used for personal financial or tax advice.

## Feedback

Found a mistake or have an idea? Use the [feedback form](https://docs.google.com/forms/d/e/1FAIpQLSen8tOrDVLJdkpFpjhgKqawVwHMIy0JHeH_Q8XEy8JMrlayGw/viewform).

## Run locally

Open `index.html` in any browser.

## Disclaimer

Interest rates change often; check current rates with your bank before you rely on them. Tax (such as capital gains tax, tax on interest and tax on rent) and bank fees are not included; please seek your own tax advice. House prices, rents and share returns are steady yearly guesses; real ones go up and down. This is for learning only and is not financial or tax advice. Seek professional services before making any commitment. Everything here is speculative and subject to change.
