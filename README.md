# The Real Cost of Investment Fees: open data (2026)

Open data behind the Eliyate Finance study **The Real Cost of Investment Fees**
(https://eliyatefinance.online/data-lab/fee-study-2026/), plus the 29 fee-cost scenarios
(https://eliyatefinance.online/data-lab/fee-cost/).

## Files

| File | What it contains |
|---|---|
| `fund_fee_benchmarks.csv` | Published average fund fees (ICI 2025, Morningstar 2024, ETF.com) with the year and the source URL. |
| `fee_study_2026_scenarios.csv` | Ending balance and dollars lost for $300 a month at 7 fee levels over 10, 20 and 30 years. |
| `fee_grid.csv` | 220 rows: 11 fee levels x 5 monthly amounts ($100 to $1,000) x 4 horizons (10 to 40 years). |
| `fee_cost_scenarios.csv` | The 29 scenarios published on the fee-cost pages, each with its page URL. |

## Model

Monthly contributions; gross return 7% a year; the yearly fee is subtracted from the return and applied monthly:
`balance = balance * (1 + 0.07/12 - fee/12) + contribution`. Contributions are made at the end of each month.
"Lost" is measured against a 0.03% fee (the largest S&P 500 index ETFs) in the study files, and against 0.10% in `fee_cost_scenarios.csv`.
All balances are hypothetical illustrations, not forecasts. Real returns vary and are not guaranteed.

## Sources of the benchmark figures

- Investment Company Institute, *Mutual Fund and ETF Fees Remained Near Historic Lows in 2025* (March 2026).
- Morningstar U.S. Fund Fee Study 2024, as reported by ETF.com.
- ETF.com, VOO vs SPY vs IVV (2026).

Fund fees change. Check a fund's current expense ratio in its prospectus before investing. Educational use only, not investment advice.

## License and citation

DOI: [10.5281/zenodo.23694700](https://doi.org/10.5281/zenodo.23694700)

Data and calculations: CC BY 4.0. Please cite:

> Eliyate Finance (2026). The Real Cost of Investment Fees: open data. https://eliyatefinance.online/data-lab/fee-study-2026/

Author: Raphael, Eliyate Finance.
