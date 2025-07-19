# Rerate Impact Analysis Model – Forecasting State-Level Auto Insurance Adjustments

This project forecasts the long-term impact of insurance rerate policies at the state level. It models how rerate adjustments play out over time using historical data and Monte Carlo simulation.

## 🎯 Objective

To estimate the future financial and operational impact of auto policy rerate cycles, enabling better rollout strategies and risk planning.

## 📁 Dataset

- Proprietary insurance rerate dataset (2015–2023)
- Includes rerate amount, date, state, policy group, risk tier, and capture status

## 🔧 Tools & Libraries

- `pandas`, `numpy` for data wrangling and simulations  
- `matplotlib`, `seaborn` for historical trends  
- `random` for stochastic simulation modeling

## 🔬 Key Techniques

- State grouping by original and proposed rollout strategies  
- 8-year Monte Carlo simulations to estimate projected rerates  
- Scenario modeling of lookback windows, capture rates, and group reassignment  
- KPI summaries and boxplot outlier detection

## 📊 Key Outputs

- Projected refund volume by year and location  
- Group-level summary statistics (mean, std dev, min, max)  
- State rollout impact and sensitivity to lookback horizon  
- Visualizations: Line plots, histograms, Monte Carlo simulations, KPI dashboards

## ▶️ How to Run

1. Open the notebook and load the provided rerate dataset.  
2. Adjust simulation parameters (lookback, grouping) as needed.  
3. Run all cells to generate projected refund amounts through 2033.  
4. Results are output as interactive visuals and summary data tables.
