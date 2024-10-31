# Movie Recommendation System

A content-based movie recommendation system built using Python, pandas, and various libraries for data processing and machine learning. This project recommends movies based on their similarities in genres, cast, crew, keywords, and overview.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Example](#example)
- [License](#license)

## Overview

This Movie Recommendation System uses data from the TMDB (The Movie Database) to recommend similar movies based on user input. The system leverages natural language processing (NLP) techniques to analyze movie descriptions and features.

## Dataset

The project utilizes two datasets:

1. **tmdb_5000_credits.csv**: Contains information about the cast and crew of movies.
2. **tmdb_5000_movies.csv**: Contains metadata about movies, including titles, budgets, genres, keywords, and overviews.

## Features

- **Movie Similarity**: Recommends movies based on the similarity of their attributes.
- **Natural Language Processing**: Processes and analyzes textual data to improve recommendations.
- **Customizable**: Easily extendable to include more features or different datasets.

## Installation

To run this project, you need to have Python installed on your machine. You can clone this repository and install the required libraries using pip.

```bash
git clone https://github.com/SamiUllah568/Movie_Recommendation_System.git
cd Movie_Recommendation_System

## **Usage**

Import the necessary libraries and load the datasets:

```python
import pandas as pd


Load the Data:
data_credit = pd.read_csv("tmdb_5000_credits.csv")
data_movies = pd.read_csv("tmdb_5000_movies.csv")


Run the recommendation function by providing a movie title

recommend("Batman Begins")

How It Works
Data Preparation: The datasets are merged and cleaned to retain relevant features.

Text Preprocessing: The text data is processed to create a tags column that combines important attributes.

Vectorization: The tags column is vectorized using the Bag of Words (BoW) method.

Similarity Calculation: Cosine similarity is calculated between movie vectors to find similar movies.

Recommendation: A function retrieves and displays the top similar movies based on user input.
**Example**
To recommend movies similar to "Batman Begins"
recommend("Batman Begins")

**Output:**
The Dark Knight
Batman
Batman
The Dark Knight Rises
10th & Wolf
