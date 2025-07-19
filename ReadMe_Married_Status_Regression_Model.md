# Married Status Regression Model

This regression project predicts whether an individual is married based on demographic and socioeconomic features. It applies logistic regression to evaluate probability outcomes and model accuracy.

## 🎯 Objective

To estimate the likelihood of marital status based on inputs such as income, age, education, employment, and household structure.

## 📁 Dataset

- CSV dataset of anonymized individuals with attributes including:
  - Age, income, education, employment status, housing type
  - Target variable: Married vs. Not Married

## 🔧 Tools & Libraries

- `pandas`, `numpy` for data loading and wrangling  
- `statsmodels` for logistic regression modeling  
- `seaborn`, `matplotlib` for EDA and visualization

## 🔬 Key Techniques

- Dummy variable encoding  
- Logistic regression with `Logit()`  
- Summary statistics and p-values for coefficient analysis  
- Confusion matrix and classification report

## 📊 Key Outputs

- Model summary table with coefficients and significance  
- Accuracy score and prediction classification  
- Interpretable output on which variables drive marriage likelihood

## ▶️ How to Run

1. Open the notebook in Jupyter or any Python IDE  
2. Run all cells in sequence  
3. Model output will print prediction accuracy and variable weights
