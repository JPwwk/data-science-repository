# Climate Dataset Exploration – Socioeconomic & Disaster Vulnerability Analysis

This project explores how state-level climate disaster exposure intersects with social vulnerability indicators to form patterns of climate equity risk. The goal is to identify state groupings using unsupervised learning.

## 🎯 Objective

To examine patterns in disaster frequency and impact by linking climate data with socioeconomic indicators, ultimately developing an equity risk index.

## 📁 Datasets

- FEMA Disaster Declarations Summary (1980–2024)
- NOAA Billion-Dollar Weather and Climate Disasters
- CDC Social Vulnerability Index (SVI 2022)
- U.S. Census QuickFacts (Population, Income)

## 🔧 Tools & Libraries

- `pandas`, `plotly.express` for processing and visualization  
- `sklearn.preprocessing`, `sklearn.cluster`, `sklearn.decomposition` for modeling  
- `matplotlib`, `seaborn` for basic EDA

## 🔬 Key Techniques

- PCA to reduce disaster metric dimensionality
- KMeans clustering of state-level disaster profiles
- Normalization of population, income, and insurance coverage
- Choropleth and radar visualizations of cluster features

## 📊 Key Outputs

- PCA plots of climate exposure profiles
- Clustered state groupings by disaster risk
- Radar plots of cluster characteristics
- Normalized Equity Risk Score = Disasters × SVI × Uninsured Rate

## ▶️ How to Run

1. Ensure all `.csv` files are in the notebook folder.  
2. Run all cells in order (EDA → PCA → Clustering → Visualization).  
3. Final equity scores are exported to `equity_index_output.csv`.
