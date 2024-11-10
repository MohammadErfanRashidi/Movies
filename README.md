# Movie Recommendation System

This project implements a content-based movie recommendation system using Python and the scikit-learn library. The system recommends similar movies based on features such as genre, keywords, tagline, cast, and director.

## How it Works

1. **Data Loading:** The system loads movie data from a CSV file named 'movies.csv'.
2. **Feature Selection:** It selects five important features: 'genres', 'keywords', 'tagline', 'cast', and 'director'.
3. **Data Preprocessing:** Missing values in the selected features are replaced with empty strings.
4. **Feature Combination:** The selected features are combined into a single text feature for each movie.
5. **Feature Vectorization:** The combined text features are converted into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.
6. **Similarity Calculation:** Cosine similarity is used to calculate the similarity between movie vectors.
7. **Recommendation:** When a user inputs a movie title, the system finds the closest match in the dataset and recommends movies with the highest similarity scores.

## Usage

1. Run all the cells in the provided Jupyter Notebook.
2. Enter the name of your favorite movie when prompted.
3. The system will output a list of recommended movies.

## Dependencies

* Python 3
* pandas
* scikit-learn
* difflib
* numpy

## Dataset

The system uses a movie dataset (movies.csv) containing information about movies, including title, genres, keywords, tagline, cast, and director.

## Note

The accuracy of the recommendations depends on the quality and completeness of the movie dataset.
