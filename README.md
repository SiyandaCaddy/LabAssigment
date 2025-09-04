# LabAssigment

Movie Recommendation System

This project implements a simple recommender system using both Collaborative Filtering and Content-Based Filtering methods. It was developed as part of Lab Assignment 1.

📂 Files

LabAssignment1.ipynb — Jupyter Notebook containing all code and results.

movies.csv — dataset of user ratings and movie metadata.

📊 Dataset

The dataset (movies.csv) contains the following columns:

user_id — unique identifier for each user.

movie_title — title of the movie.

rating — rating given by the user (1–5 scale).

genre (optional) — one or more genres for each movie, separated by |.

Example:

user_id;movie_title;rating;genre
1;The Matrix;5;Action|Sci-Fi
1;Titanic;4;Romance|Drama
2;The Matrix;4;Action|Sci-Fi
2;Avatar;5;Action|Adventure|Sci-Fi

⚙️ Methods Implemented
1. Collaborative Filtering

Builds a user–item matrix from ratings.

Computes cosine similarity between users.

Recommends movies by finding the most similar user to the target user.

2. Content-Based Filtering

Uses movie genres as features.

Applies CountVectorizer to convert genres into vectors.

Computes cosine similarity between movies.

Recommends movies similar to those highly rated by the target user.

▶️ How to Run

Upload movies.csv into Colab:

from google.colab import files
uploaded = files.upload()


Run all cells in LabAssignment1.ipynb.

When prompted, enter a user_id to generate recommendations.

📌 Deliverables

Dataset: movies.csv

Notebook/Script: LabAssignment1.ipynb

Reflection:

Which method (Collaborative vs Content-Based) gave better recommendations?

What challenges did you face (e.g., missing data, cold-start users)?

How might this system be improved (e.g., hybrid models, larger datasets)?

🚀 Extensions

Implement a Hybrid Recommender (combine collaborative + content-based).

Test on a larger dataset like MovieLens
.

Add features like year, director, or actors for richer content-based filtering.
