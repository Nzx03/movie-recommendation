# **Movie Recommendation System**

## **Overview**
This project is designed to recommend movies to users based on textual data such as movie overviews, genres, cast, keywords, and crew information. By leveraging libraries like `numpy`, `pandas`, `scikit-learn`, `difflib`, and `ast`, the system provides personalized movie suggestions using advanced vectorization and similarity computation techniques.

## **Features**
- **Data Merging**: Combines multiple datasets based on a common column (`title`) for a unified dataset.
- **Data Cleaning**: Handles missing data and removes unnecessary columns for better processing.
- **Data Transformation**:
  - Converts string representations of lists into Python lists using the `ast` module.
  - Extracts the director's name from the `crew` column for more accurate recommendations.
- **Text Normalization**: 
  - Converts all text to lowercase.
  - Replaces spaces with underscores for uniformity.
  - Combines relevant columns (e.g., `overview`, `keywords`, `genres`, `cast`, and `crew`) into a single `tag` column.
- **Vectorization**: Converts textual data into numerical format using **TF-IDF Vectorization**.
- **Cosine Similarity**: Measures the similarity between feature vectors to find the most similar movies.
- **Error Handling with difflib**: Corrects user input spelling errors and suggests the closest matching movie titles.
- **Top 10 Recommendations**: Provides a ranked list of 10 movies similar to the user-provided input.

---

## **Technologies Used**
- **Python**: Programming language used for the implementation.
- **NumPy**: For efficient numerical computations.
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For TF-IDF vectorization and cosine similarity calculations.
- **Difflib**: For matching user input to movie titles.
- **AST**: For parsing and evaluating string representations of lists.

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
