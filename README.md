# Netflix FP&A Model & Variance Analysis

A driver-based revenue forecast, scenario model, and quarterly variance analysis for Netflix, built entirely from public SEC filings (8-K shareholder letters, 10-Qs, 10-K).

## Business Question

How would an internal FP&A team forecast Netflix's revenue and operating income by region, and how should that forecast be revised once actual results come in?

## Method

- **Revenue Build:** Regional revenue (UCAN, EMEA, LATAM, APAC) modeled off YoY growth rates rather than subscriber × ARPU, since Netflix discontinued regional subscriber/ARPU disclosure after Q3 2025. The model adapts to that reporting change rather than forcing stale inputs.
- **Historical tab:** 21 quarters of actuals (Q1'21 to Q1'26) sourced directly from filings, adjusted for Netflix's November 2025 10-for-1 stock split, with a one-time $2.8B non-operating item (the Warner Bros. Discovery merger termination fee, Q1'26), flagged separately so it doesn't distort operating trends.
- **Scenario tab:** Base/Bull/Bear toggle for growth and margin assumptions, feeding directly into the Revenue Build and P&L tabs.
- **Variance tab:** Compares the Base-case forecast to Netflix's actual Q2'26 results (reported July 16, 2026), with a full revenue-by-region bridge and an operating income bridge separating the revenue effect from the margin effect.

## Headline Finding: Q2'26 Forecast vs. Actual

| | Forecast (Base) | Actual | Variance |
|---|---|---|---|
| Total Revenue | $12,707M | $12,560M | ($147M), -1.2% |
| Operating Margin | 30.0% | 33.4% | +3.4pp |
| Operating Income | $3,812M | $4,193M | +$381M, +10.0% |

Revenue missed across UCAN, EMEA, and APAC, and was only partly offset by LATAM outperforming (+3.6%, the second straight quarter LATAM beat forecast). Despite the revenue miss, operating income beat by $381M, and the bridge shows that beat came **entirely from margin, not revenue**. The revenue shortfall cost about $44M of profit, while margin outperformance added $425M, netting the full $381M beat.

## Recommendation

1. **Don't carry the 33.4% margin forward.** Netflix's own shareholder letter attributes the beat to favorable expense timing, not a structural improvement. Q3'26–Q1'27 margin assumptions should stay near the trailing average rather than being raised off one strong quarter.
2. **Revisit UCAN and APAC growth assumptions.** Both regions have missed forecast by a widening margin for several quarters running. This reads as a persistent trend, not a one-off miss, and should be reflected in the Q3'26 forecast.
3. **Hold or raise the LATAM growth assumption.** LATAM is now two-for-two beating forecast and remains the fastest-growing region.

## Files

- `netflix_fpa_model.xlsx`: full model (Cover, Assumptions, Historical, Revenue Build, P&L, Scenario, Variance, Dashboard tabs)
- `Q2_26_Variance_Memo.pdf`: full written variance memo

## Sources

Netflix Inc. 8-K shareholder letters, 10-Q, and 10-K filings, SEC EDGAR.
