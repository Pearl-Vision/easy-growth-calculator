# Easy Growth Planner

**Compare. Plan. Grow.** A compound interest planner that runs in the browser. It needs no install and no build step.

**Live app:** https://pearl-vision.github.io/easy-growth-calculator/

## What it does

- Enter a starting amount, a regular contribution (monthly, quarterly, half-yearly or yearly), a yearly interest rate and how often interest compounds (daily, monthly, quarterly, half-yearly or yearly). Compounding starts on yearly.
- When the page opens, Options A, B and C show **example numbers in your own money**: 10,000 US dollars to start and 500 a month, changed into your currency at today's exchange rate and rounded (for example A$15,000 and A$740), at 6% (A), 8% (B) and 4% (C) a year for 20 years. The Goal finder starts with an example goal of 100,000 US dollars in your money (for example A$150,000). Type your own numbers over them, or press **clear them** to start from 0. The page starts fresh each time it opens.
- Choose a period of 1 to 50 years.
- Add inflation, either one rate for every year or a different rate for each year, to see the final value in today's money.
- See the results in summary tiles, a stacked growth chart and a year-by-year table.

## Compare options

- **Option A** is your main details.
- **Options B and C** are laid out exactly like Option A. Each has its own currency, starting amount, contribution, rate, compounding, inflation (the same as A, or their own rate) and number of years ("Same as Option A", or its own 1 to 50 years). When options run for different numbers of years, the tables and chart go up to the longest one, an option shows "—" after it ends, and each final value is at the end of that option's own years. Option D uses Option A's years.
- **Different currencies:** Option A's currency is your local currency. If Option B or C uses another currency, today's exchange rate is filled in for you (from [ExchangeRate-API](https://www.exchangerate-api.com), which publishes new rates once a day); you can type your own rate instead. The page fetches the new day's rates by itself as soon as they are published, even if it stays open, and shows the date of the rate it is using. If the service can't be reached, it keeps the last rate and tries again every 10 minutes. All comparisons use your local currency, and a **Totals in your local currency** table shows each option's currency, the rate, the final value in its own currency and in your local currency. The rate is assumed to stay the same for the whole period.
- **Option D** is either **buying a house** with a loan or **investing in shares**:
  - House: first choose **home to live in (PPR)** or **investment property**. Then enter the price, deposit, buying costs, yearly costs, loan term, house value growth and a loan rate that is fixed or changes each year (the repayment is worked out again when the rate changes). The final value is your equity: the house value minus the loan still owed.
  - Investment property also takes the weekly rent (with a yearly increase) and selling costs. Rent received lowers the money you put in, and selling costs come off the house value. Tax is not included.
  - Shares: starting amount, contribution, expected return and compounding. For **rent vs buy**, add the rent you would pay if not buying (with a yearly increase); it counts as money spent and does not grow. **Use the same money as the house** invests what is left after rent, so both put in the same total.
  - Option D can use Option A's inflation or its own.
- When you compare, the top card shows the **winner** (the biggest final value). The comparison shows a summary table, a chart you can switch between lines, bars, shaded areas and the difference from Option A, and year-by-year balances. The main year-by-year table adds columns for each option.

## Page layout

0. **How to use**: four animated steps (Fill in Option A, Compare, Set a goal, See the winner). Click a step to jump there. The ✕ hides it (remembered in your browser); "❔ How to use" brings it back. The **▶ Watch the 1-minute guide** button opens `guide.html`, an animated cartoon guide starring EGP the coin (seven short scenes with Back, Next and Pause). Press **💰 Money sounds** for a cash-register "ka-ching" and coin clinks at the big moments (the money waterfall, KA-CHING!, each option reaching the goal, the winner's trophy), and **🎵 Music** for an original tune. All sound is made live by the page; there are no sound files.
1. Results at the top: the **Year by year balances** chart (always shown, one line per option) beside the main results card.
2. The four options side by side: Option A (your details) on the left, then Options B, C and D, always open and the same height. The **Goal finder** (see below) sits under Options B, C and D.
3. **Compare your options** beside the **Year by year** table.

Options B, C and D are left out of the comparison until you type a starting amount or a contribution (for a house, a price or deposit). On a tablet the options show two by two with the Goal finder under them; on a phone everything is in one column.

## Goal finder

- Type a goal (in future money, or in today's money allowing for inflation). For Option A, and for Options B and C once you use them, it shows how much to add each time to reach the goal in your chosen years (with a button to use that amount in that option) and how long it takes with what you add now. Each option uses its own settings. It also says which option reaches the goal first.
- On the **Year by year balances** chart (Lines, Bars or Shaded areas), an outlined bar in each option's colour, with the 🎯 Goal finder symbol inside, marks the year it reaches the goal with what it adds now, as tall as its balance that year. A note under the chart lists what each option has and when.
- The goal is in your local currency. For an option in another currency, the goal and the amounts are shown in that currency, with the local amount next to them.

## Currencies

- Pick from 9 currencies, or type any other currency. The page picks a starting currency for any country in the world: it works out the country from the device's time zone (for example Asia/Kuala_Lumpur means Malaysia, so Malaysian Ringgit), or else from the device's language and region setting. It reads these from the device and does not send them anywhere. Your last currency choice is remembered in your own browser only.
- You type your own interest rates. Check current rates with your bank or a comparison website.

## Privacy

- Visits are counted anonymously with [GoatCounter](https://www.goatcounter.com/): no cookies and no personal data. It records only things like the page visited, the country, the type of device and where the visit came from.
- The amounts, rates and other numbers you type never leave your browser.
- The page asks ExchangeRate-API for today's rates when it opens outside the USA (to show the example numbers in your money) and when Option B or C uses a different currency. It sends only a currency code (for example AUD).
- Opening `index.html` from your own computer is not counted.
- The **Feedback / Contact** link opens a separate Google Form. Only what you choose to type there is sent (your email is optional), and Google stores it. The form is not used for personal financial or tax advice.

## Feedback

Found a mistake or have an idea? Use the [feedback form](https://docs.google.com/forms/d/e/1FAIpQLSen8tOrDVLJdkpFpjhgKqawVwHMIy0JHeH_Q8XEy8JMrlayGw/viewform).

## Run locally

Open `index.html` in any browser.

## Disclaimer

Interest rates change often; check current rates with your bank before you rely on them. Tax (such as capital gains tax, tax on interest and tax on rent) and bank fees are not included; please seek your own tax advice. House prices, rents and share returns are steady yearly guesses; real ones go up and down. This is for learning only and is not financial or tax advice. Seek professional services before making any commitment. Everything here is speculative and subject to change.
