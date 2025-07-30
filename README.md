# RetailProductRecommendationSystem

This repository contains an item-based collaborative filtering recommendation system for retail products built with Python. The project uses Amazon review data from 7817_1.csv.

## Features

- Loads and pre-processes a real-world Amazon reviews file (7817_1.csv)
- Selects relevant columns: user_id, product (asins), and rating (reviews.rating)
- Handles missing/invalid data and keeps only usable ratings
- Samples data for memory efficiency, so it runs in Google Colab or on laptops
- Builds a user-product ratings matrix for collaborative filtering
- Computes product similarity using cosine similarity
- Provides personalized top-N product recommendations for any user in the sample
- Includes simple visualizations: top-rated and most-rated sample products

## How to Run

1. Place 7817_1.csv in your working directory or upload it to Google Colab.
2. Run the notebook script with the provided code (see main.ipynb).
3. The script automatically samples up to 1,000 users and 100 products (adjustable based on your dataset size).
4. Use the recommend_products(user_id, pivot, sim_df, top_n) function to get recommendations. Example usage is shown in the code.
5. The notebook will also show simple bar plots for the sample's top products.

## Requirements

- Python ≥ 3.7
- pandas
- numpy
- scikit-learn
- matplotlib
