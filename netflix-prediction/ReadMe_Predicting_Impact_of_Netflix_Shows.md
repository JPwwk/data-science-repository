# Predicting Impact of Netflix Shows

This project explores what makes a Netflix series successful in terms of longevity and viewer engagement. It analyzes show metadata and streaming statistics to identify key predictors of impact.

## 🎯 Objective

To identify features that correlate with the success and viewer retention of Netflix titles, such as runtime, release timing, and genre.

## 📁 Dataset

- Netflix Top 10 titles (weekly data)
- Includes: genre, title, hours viewed, weeks in top 10, runtime, release year

## 🔧 Tools & Libraries

- `pandas`, `numpy` for data prep  
- `matplotlib`, `seaborn`, `plotly` for visualization  
- `scikit-learn` for exploratory modeling

## 🔬 Key Techniques

- Runtime segmentation analysis  
- Scatterplots of hours viewed vs. weeks charted  
- Logistic regression classification on top performers  
- Violin plots of duration and performance

## 📊 Key Outputs

- Visual trends on title popularity and duration  
- Highlighted outliers (e.g., series that stayed charted unusually long)  
- Basic predictive model for viewer engagement

## ▶️ How to Run

1. Open the Jupyter Notebook  
2. Ensure the dataset is in the working directory  
3. Run all cells to generate visualizations and modeling output
