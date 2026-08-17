# Buy vs Rent — GTA Comparison

A free, open-source calculator that compares the **total cost of buying versus renting the same home** in the Greater Toronto Area — mortgage, taxes, fees, appreciation, and the investment you'd make instead of buying.

**🔗 Use it here: https://sanatchugh.github.io/buy-vs-rent-gta/**

![License: MIT](https://img.shields.io/badge/license-MIT-green)

---

## What it is

"Should I rent or buy?" usually gets answered with a rule of thumb, or a simple monthly-payment-vs-rent comparison — both of which leave out most of the picture. A real answer has to account for the down payment, closing costs (land transfer tax, CMHC insurance), property tax, condo fees or upkeep, insurance, selling costs, home appreciation, rent inflation, **and** the return you'd earn by investing your money instead of tying it up in a home.

This calculator puts all of that in one place, turns every assumption into something you control, and shows the year-by-year outcome of each path — including the exact year (if any) that buying overtakes renting.

It's deliberately **neutral**: it makes no recommendation. It shows the numbers; you decide.

## What it's looking to achieve

- Give GTA renters and buyers an honest, complete comparison instead of an oversimplified one.
- Make the hidden costs of buying — and the opportunity cost of the down payment — visible and adjustable.
- Let you stress-test the assumptions that actually decide the answer (home appreciation and investment return), so you can see your downside before committing.

## How to use it

Open the site and work down the panel on the left. As you change any figure, the results on the right update instantly. It opens in **Simple** mode — just the essentials (price, down payment, location, property type, rent, horizon), with every other assumption pre-filled from real GTA data and tucked into collapsible groups that show what they assume. Flip to **Advanced** to expand everything. On a phone, the verdict and chart appear first, above the inputs.

0. **(Optional) Start from a preset** — the **Quick start** buttons load a typical GTA scenario (first-time condo in the 416, a 905 townhouse, a Toronto semi, a 905 detached) so you're not staring at a blank slate. Then adjust anything below.
1. **Describe the place** — purchase price, how much you can put down, location (905 vs Toronto/416), and property type. The tool flags if your down payment is below the legal minimum or your upfront cash exceeds your budget.
2. **Set your assumptions** — mortgage rate (with a separate renewal rate for year 6+), property tax, condo fees or upkeep, insurance, home appreciation, rent, and rent growth. Each field shows how fast that cost has actually grown over the past 1–20 years, so your inputs aren't guesses.
3. **Set the investment alternative** — how much you'd invest each year if you rented instead, your expected return, and the tax on gains.
4. **Read the results:**
   - The **verdict** — who is ahead at your chosen horizon, and by how much.
   - The **crossover year** — when (if ever) buying pulls ahead of renting.
   - The **net-worth chart** — both paths over 30 years; hover (or tap, on mobile) any year to inspect it.
   - **How the answer changes** — the **break-even appreciation rate** (the growth at which buying exactly ties renting) plus a **sensitivity grid** showing the verdict across a range of appreciation × investment return, so you see the whole decision space at once.
   - The **monthly** and **upfront cash** breakdowns, and a **year-by-year** table.
5. **Stress-test it** — set appreciation to 0% and −2% to see the downside, and try different investment returns. This is where the real decision lives.
6. **Compare two options** — pin any setup as **A**, change your inputs, pin **B**, and see them side by side (buy now vs wait, condo vs detached, 5% vs 20% down).

Your numbers never leave your browser — nothing is uploaded, stored, or tracked.

## How the comparison works

Both paths start with the same cash. The buyer puts it into the **down payment + closing costs**; the renter invests it. Going forward, the renter also invests the difference between owning and renting. You can do this two ways: a **fixed amount** each year (defaulted to the own-minus-rent gap), or the **actual yearly gap** — the real month-by-month difference on whichever side is cheaper that year (the renter while owning costs more; the buyer once it costs less). The actual-gap mode is the fairer both-sides comparison, since a fixed amount overstates the renter's savings once rent outgrows the fixed mortgage payment.

At your chosen horizon the tool compares:

| Path | Net worth =                                                        |
|------|-------------------------------------------------------------------|
| Buy  | Home value − mortgage balance − selling costs (**tax-free** as a principal residence) |
| Rent | Invested contributions grown at your return − tax on the gains + deposit returned |

Mortgage **principal isn't treated as a cost** — it lowers your balance and becomes equity at sale, so the "forced savings" of a mortgage are counted fairly.

## What it accounts for

**You control:** purchase price, down payment, location (905 vs Toronto/416), property type, first-time-buyer status, mortgage rate (years 1–5 and 6+), amortization, property tax, condo fees / upkeep, insurance, appreciation, selling costs, legal fees, rent, rent growth, tenant insurance, annual investment amount, investment return, tax on gains, horizon, and upfront budget.

**Built in automatically** (kept out of the inputs to reduce clutter — all shown in the tool's notes):

| Assumption | Value |
|---|---|
| One-time moving cost (on purchase) | $1,500 |
| Condo special-assessment reserve (condo types) | $50 / month |
| CMHC surcharge for 30-year insured amortization | +0.20% of the loan |
| Last-month-rent deposit | 1 month's rent (returned, earns nothing) |
| Purchase type | Resale (no new-build HST) |
| Utilities | Excluded on both sides (a cost-of-living item) |

Ontario + Toronto land transfer tax, first-time-buyer rebates, CMHC insurance tiers, and the minimum-down-payment rules are all built in.

## Historical averages built into the tool

Approximate annual increases for the Toronto/GTA area, rounded from public data. These populate the note under each field so your growth assumptions start from reality:

| Cost | ~20y | ~10y | ~5y | ~3y | ~1y |
|---|---|---|---|---|---|
| Property tax (Toronto) | ~3% | ~4% | ~5% | ~6% | ~2% (2026) |
| Condo fees | ~3% | ~3.5% | ~3.7% | ~3.7% | ~4% |
| Home insurance (Ontario) | ~5% | ~6.3% | ~7% | ~7% | +7.2% (2025) |
| Home price | ~+6% | ~+4.6% | ~+2% | ~−3% | ~−4.5% |
| Rent (Toronto) | ~+3.5% | ~+4.5% | ~+3% | ~+1% | 3-bed +3.9% |

Property tax spiked 9.5% in 2024 and 6.9% in 2025. Home prices are strongly up long-term but in a correction as of 2026 — which is exactly why appreciation is the single most important assumption to stress-test.

## Limitations — where this can go wrong

The result is only as good as its two biggest assumptions: **home appreciation** and **investment return**. Small changes swing the answer a lot.

> **Example:** a $900k home at 3%/yr is worth ~$1.04M in 5 years. But GTA prices fell ~4.5% in the last year. If they instead drop 2%/yr for 5 years, that home is worth ~$813k — a ~$230k swing that turns a 5-year "buying ahead" into "renting clearly ahead."

Always run the numbers at 0% and −2% appreciation before deciding. Other simplifications: property assessments are assumed to track price; new-build HST and rebates aren't modelled; individual mortgage/tax edge cases and condo special assessments (beyond the flat reserve) aren't captured; and 905 property-tax rates vary by municipality.

## Data sources

Figures and defaults are drawn from public data including the Toronto Regional Real Estate Board (TRREB), the City of Toronto, the Ontario Ministry of Finance (land transfer tax), CMHC, MyChoice / insurance industry reporting, Rentals.ca, RE/MAX, and WOWA. Rates and defaults reflect an **August 2026 baseline** and should be verified before you rely on them.

## Disclaimer

This is a decision aid, **not financial, tax, or legal advice.** The figures are estimates you control and may not reflect your situation. Verify current rates, taxes, and rebates — and consider speaking with a licensed mortgage broker, financial planner, or real estate lawyer — before making a decision.

## Authors

- **Sanat Chugh** — [github.com/sanatchugh](https://github.com/sanatchugh)
- **Claude** (Anthropic)

## License

Released under the [MIT License](./LICENSE).
