# Bachelor-Thesis-ECB-Upload
Bachelor Thesis for ECB application "Traineeship Forecasting and Policy Modelling": 

Carbon Tariffs in Practice: A Structural Gravity Analysis of the European Carbon Border Adjustment Mechanism


I extended a structural gravity model to mirror EU-ETS policy rules to study how free allocation and CBAM interact during the 2026–2034 transition period. The model has an Eaton-Kortum-type structure with an internationally traded fossil resource building on Larch and Wanner (2024). The model uses GTAP 11 data (2017) with 159 countries and 13 tradable sectors. 
My core contribution is adding EU climate policies in the model: (i) a carbon tax with endogenous price adaptation to hit the 62% reduction target covering only EU-ETS sectors; (ii) a free allocation subsidy modelled as indirect income stream separate from the carbon tax; (iii) a CBAM-like carbon tariff for regulated goods, determined by the imported good’s carbon intensity and reduced by the amount of free allocation the good faces in the EU.
I implemented two shocks to isolate the CBAM effect: first carbon pricing with free allocation, to move the 2017 baseline to the 2024 level; then CBAM with free allocation faded to its 2030 rate and the 2030 target.
From facility-level EU Transaction Log data (free and surrendered permits, industry) I computed country-sector free allocation shares, clustering countries for enough observations per cell and trimming the top decile of ratios (robust to alternative cut-offs).
Carbon tariffs need a price correction factor because the model works with value shares while the EU framework counts tons. From BACI trade flows (quantity and value, HS6, 200 countries) I reconstruct prices and build country-pair-sector price ratios.I prepared the data in R and solved the model numerically in GAMS.
The CBAM and free allocation phase-out shock leads to a carbon leakage rate around 0 (slightly negative unlike comparable studies). Tariffs of about 12-24% for emission-intensive exporters decrease their EU trade shares lowering domestic production. Real income losses are small (below 0.2%). The numerical results are preliminary lacking robustness checks and scenario comparisons.
