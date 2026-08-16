# ExxonMobil DCF Valuation

A discounted cash flow model estimating ExxonMobil's fair value, cross-checked against relative valuation versus Chevron and Shell, with a full written investment thesis.

## Business Question

Is ExxonMobil stock worth what it is currently trading at, based on the cash the business is expected to generate?

## Method

A five-year discounted cash flow model:

- Estimate free cash flow for each of the next five years, based on revenue growth, EBIT margin, and CapEx assumptions
- Discount those cash flows to present value using a WACC of 8.20% (CAPM-based cost of equity plus after-tax cost of debt, at target capital structure)
- Add a terminal value beyond year five, using a 2.50% long-run terminal growth rate
- Subtract debt, add back cash, and divide by shares outstanding to arrive at fair value per share

| Driver | Assumption | Rationale |
|---|---|---|
| Revenue Growth | 2.0% to 3.0% over 5 years | Production growth (Permian, Guyana) offsetting flat-to-soft commodity prices |
| EBIT Margin | 13.0% to 14.5% | Gradual recovery from 2025, supported by structural cost savings |
| CapEx (% of sales) | 8.5% to 7.5%, tapering | Management guidance of $27 to 29B, flattening as growth projects complete |
| WACC | 8.20% | CAPM-based cost of equity plus after-tax cost of debt |
| Terminal Growth | 2.50% | Roughly long-run GDP and inflation |

## Headline Finding

The model estimates ExxonMobil's fair value at approximately **$132 per share**, below the trading price. A relative valuation cross-check against Chevron and Shell (using price-to-earnings multiples and dividend yield) points to the same conclusion:

| Company | P/E (years of profit paid for) | Dividend Yield |
|---|---|---|
| ExxonMobil (XOM) | ~20.6x | ~2.6% |
| Chevron (CVX) | ~18.9x | ~3.6% |
| Shell (SHEL) | ~12.4x | ~3.5% |

ExxonMobil is the most expensive of the three on this measure and pays the smallest share of its stock price as a dividend, consistent with the DCF's read that the stock is priced at a premium.

Sensitivity matters here: adjusting the discount rate and terminal growth rate alone swings the estimate from $98 to $201 per share. The conclusion is best read as "overpriced under reasonable, middle-of-the-road assumptions," not as a precise target.

## Context

As of August 2026, the war in the Middle East and the resulting disruption to Strait of Hormuz shipping is the single largest near-term factor for ExxonMobil, larger than any modeling assumption in this analysis. Higher oil prices from the disruption support the model's profit assumptions in the near term, but the situation is fluid and could reverse quickly with a peace deal, or intensify further.

## Bottom Line

ExxonMobil's stock appears overpriced relative to the cash the business is likely to generate, with two independent methods (DCF and relative valuation) pointing the same direction. The size of the gap is genuinely uncertain given the unresolved conflict currently driving oil prices, and the market may simply be paying a fair price for ExxonMobil's stability and track record rather than mispricing the stock.

## Files

- `exxonmobil-dcf-model.xlsb`: full DCF and comparables model
- `exxonmobil-investment-thesis.pdf`: full written investment thesis with sources

## Sources

ExxonMobil FY2025 Form 10-K and Annual Report (SEC EDGAR), U.S. Energy Information Administration Short-Term Energy Outlook (August 2026), International Energy Agency Oil Market Report (August 2026), Federal Reserve Bank of St. Louis (FRED). Full source list in the investment thesis PDF.
