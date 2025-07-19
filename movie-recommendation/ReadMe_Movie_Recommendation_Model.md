# Movie Recommendation Model

This lightweight recommendation engine uses basic string similarity techniques to return suggested movie titles based on user input. The model focuses on title-level matching without external APIs.

## 🎯 Objective

To build a simple movie recommender using title similarity and return the top-n most similar results to the viewer's query.

## 📁 Dataset

- CSV of movie titles, genres, release year, and ratings
- No third-party API or database connection required

## 🔧 Tools & Libraries

- `pandas` for data manipulation  
- `difflib` for fuzzy string matching  
- `matplotlib` for optional visual output

## 🔬 Key Techniques

- Lowercase and whitespace normalization  
- Fuzzy string scoring using `difflib.get_close_matches()`  
- User-input to dynamic top-n title return

## 📊 Key Outputs

- Top 5 movie recommendations based on string similarity  
- Optional output of genre and release year metadata  
- Easily adaptable for user interfaces

## ▶️ How to Run

1. Load the notebook in Jupyter  
2. Modify the `user_input` field with any movie title  
3. Run the notebook to return suggested titles based on fuzzy matching
