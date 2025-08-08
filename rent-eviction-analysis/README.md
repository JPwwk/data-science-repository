# Rent & Eviction Analysis — Forecasting Eviction Risk from Rental Dynamics

## Overview
This project analyzes eviction filings across U.S. ZIP codes and their relationship with rent dynamics and unemployment.  
We integrate Eviction Lab filings with Zillow rent indices (ZORI) and BLS unemployment to engineer features (rent volatility, pre‑pandemic baseline, seasonal indicators) and fit a Random Forest regression that predicts monthly eviction filings.

**Why it matters:** Eviction is highly localized and costly. Identifying high‑risk ZIPs enables targeted, early interventions.

## Data
- **Eviction Lab** — Monthly eviction filings by ZIP
- **Zillow ZORI** — Observed Rent Index (levels + volatility)
- **BLS** — Unemployment rates
- **Provided files (this repo, `/data`)**  
  - `all_sites_monthly_2020_2021_eviction.csv`  
  - `City_zori_uc_sfrcondomfr_sm_month.csv`  
  - `houston_monthly_2020_2021_eviction.csv`  
  - `main_landing_page_data.csv`  
  - `National_zorf_growth_uc_sfr_sm_month.csv`  
  - `SeriesReport-20250719175049_8a84c4.xlsx`  
  - `Zip_zori_uc_sfrcondomfr_sm_month.csv`

> Note: Some files are illustrative subsets/exports aligned to the analysis notebook.

## Methods
1. **Cleaning & Merge** — Align by ZIP and month; standardize units and date indices.  
2. **Feature Engineering** — Rent volatility, unemployment rate, pre‑pandemic filings baseline, and seasonal month indicators.  
3. **Modeling** — Random Forest Regressor.  
4. **Validation** — Group‑aware splits by ZIP (GroupShuffleSplit/GroupKFold) to avoid geographic leakage.  
5. **Evaluation** — R² and RMSE; feature importance; predicted vs. actual plots.

## Key Results
- **Top predictors:** rent volatility and the pre‑pandemic eviction baseline.  
- **Performance:** test R² ≈ 0.61 (moderate accuracy on known ZIPs); generalization to unseen ZIPs is weaker (grouped CV R² ≈ 0.10), indicating a need for local calibration.  
- **Implication:** Track volatility + history as early‑warning signals; prioritize high‑volatility/high‑baseline ZIPs for proactive support.

## Repository Structure
