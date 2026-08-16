# Netflix FP&A Model & Variance Analysis

A driver-based revenue forecast, scenario model, and quarterly variance analysis for Netflix, built from public SEC filings.

## Business Question

How would an internal FP&A team forecast Netflix's revenue and operating income by region, and how should that forecast be revised once actual results come in?

## Method

- **Revenue Build:** Regional revenue (UCAN, EMEA, LATAM, APAC) modeled off YoY growth rates, adapting to Netflix's discontinuation of regional subscriber/ARPU disclosure after Q3 2025.
- **Historical tab:** Actuals sourced directly from filings, adjusted for Netflix's November 2025 stock split, with one-time items flagged separately so they do not distort operating trends.
- **Scenario tab:** Base, Bull, and Bear toggle for growth and margin assumptions, feeding directly into the Revenue Build and P&L tabs.
- **Variance tab:** Compares the Base-case forecast to Netflix's actual Q2'26 results, with a full revenue-by-region bridge and an operating income bridge separating the revenue effect from the margin effect.

## Headline Finding: Q2'26 Forecast vs. Actual

| | Forecast (Base) | Actual | Variance |
|---|---|---|---|
| Total Revenue | $12,707M | $12,560M | ($147M), -1.2% |
| Operating Margin | 30.0% | 33.4% | +3.4pp |
| Operating Income | $3,812M | $4,193M | +$381M, +10.0% |

Revenue missed across UCAN, EMEA, and APAC, and was only partly offset by LATAM outperforming for the second straight quarter. Despite the revenue miss, operating income beat by $381M, and the bridge shows that beat came entirely from margin, not revenue. The revenue shortfall cost about $44M of profit, while margin outperformance added $425M, netting the full $381M beat.

## Recommendation

1. **Do not carry the 33.4% margin forward.** Netflix's own shareholder letter attributes the beat to favorable expense timing, not a structural improvement. Q3'26 to Q1'27 margin assumptions should stay near the trailing average rather than being raised off one strong quarter.
2. **Revisit UCAN and APAC growth assumptions.** Both regions have missed forecast by a widening margin for several quarters running. This reads as a persistent trend, not a one-off miss, and should be reflected in the Q3'26 forecast.
3. **Hold or raise the LATAM growth assumption.** LATAM is now two-for-two beating forecast and remains the fastest-growing region.

## Files

- `netflix-fpa-model.xlsx`: full model (Cover, Assumptions, Historical, Revenue Build, P&L, Scenario, Variance, Dashboard tabs)
- `q2-26-variance-memo.pdf`: full written variance memo

## Sources

Netflix Inc. 8-K shareholder letters, 10-Q, and 10-K filings, SEC EDGAR.
