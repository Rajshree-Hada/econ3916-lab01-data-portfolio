# econ3916-lab01-data-portfolio
The Data Portfolio — Big Mac Index Analysis
Objective

An applied purchasing-power-parity study using The Economist's Big Mac Index to quantify currency misvaluation across 57 economies from 2000 to 2026, with attention to data structure, missing-data mechanisms, and the limits of a single-good PPP proxy.

Methodology
Ingested the Big Mac Index directly from The Economist's public GitHub repository (57 countries, 45 reporting periods, April 2000 – July 2026; 54 countries present in the July 2024 cross-section).
Derived implied PPP exchange rates as the ratio of local-currency Big Mac price to the U.S. dollar price, then computed valuation percentages as the deviation of the implied PPP rate from the prevailing market exchange rate.
Classified the dataset along its three usable structures — cross-sectional (single reporting period, many countries), time series (single country across periods), and panel (both dimensions) — and selected slices appropriate to each research question.
Diagnosed missing-data patterns by coverage and exit date; Russia's post-2022 absence was classified as Missing Not At Random, since the withdrawal of the reporting franchise is itself correlated with the economic and political conditions the index measures.
Produced two visualizations: a ranked bar chart of currency valuation for the July 2024 cross-section, and a multi-country time series tracing valuation trajectories over the full panel.
Key Findings
The Swiss franc is persistently overvalued against the dollar on a Big Mac basis, reaching +41.8% in the July 2024 cross-section — the widest positive deviation in the sample and consistent with its standing across the broader series.
The Japanese yen is undervalued on average in every decade of the series, a durable gap rather than a cyclical one.
The divergence between the Swiss and Japanese trajectories illustrates the index's core caveat: raw Big Mac deviations conflate genuine currency misalignment with cross-country differences in labor costs, rents, and non-tradable input prices, and are best read alongside GDP-adjusted variants.
Coverage gaps are non-random and should be treated as informative rather than imputed; dropping Russia post-2022 biases any regional aggregate that includes it.
