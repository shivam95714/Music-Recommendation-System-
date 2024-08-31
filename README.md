# Song Recommender System
## Introduction
The provided code implements a Song Recommender System using a dataset containing information about songs released in the last 100 years. The dataset includes general information about songs and scientific sound metrics like loudness, acoustics, and speechiness.

## Dataset Loading and Cleaning
Imports necessary libraries and loads the dataset from 'dataset.csv'.
Conducts data cleaning steps, including handling null values and removing unnecessary columns.
Removes rows with non-English track names and eliminates information within brackets in the 'track_name' column.
Drops duplicate rows, keeping only the first occurrence of each unique set of data.
## Exploratory Data Analysis (EDA)
Examines the distribution of float-valued columns in the dataset using distribution plots.
## Feature Engineering
Incorporates the 'tags' column by combining genre and artist information for enhanced song recommendations.
Drops unnecessary columns not needed for the recommender system.
## Dataset Reduction
Due to computational constraints, limits the dataset to the top 10,000 songs based on popularity.
## Text Vectorization
Utilizes CountVectorizer to convert text data into a format suitable for machine learning algorithms.
## Similarity Calculation
Computes cosine similarity between songs based on their textual features.
The recommender system employs cosine similarity, a measure to find similar items based on feature vectors, calculated from a combination of genre and artist information using CountVectorizer. The system recommends songs by assessing similarity factors and sorting them based on popularity.
## Recommender Function
Implements a function to recommend songs based on an input song name, utilizing similarity factors.
Handles cases where the input song is not found, suggesting alternative songs from the dataset.
## Recommendation Example
Demonstrates the recommendation system by suggesting songs similar to "Khairiyat."
Handles the case where the input song is not present or not popular.
This code provides a comprehensive system for recommending songs based on textual and numeric features, enhancing user experience in discovering new music.
