# Movie Recommendation System using ML

This project is a Movie Recommendation System built using machine learning techniques. It utilizes the MovieLens 20M dataset (ml20) to generate personalized movie recommendations for users. The system is designed to demonstrate end-to-end machine learning workflows, including data preprocessing, model training, evaluation, and recommendation generation.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack and Libraries](#tech-stack-and-libraries)
- [Setup and Installation](#setup-and-installation)
- [Data Preparation](#data-preparation)
- [Models Implemented](#models-implemented)
- [Results](#results)
- [Contributing](#contributing)

---

## Project Overview

The Movie Recommendation System predicts movies that a user might like based on their past ratings and preferences. It leverages collaborative filtering and content-based filtering techniques to make relevant recommendations.

The system is built for:
- Learning and experimenting with machine learning and recommender system algorithms.
- Showcasing a reproducible data science project from data acquisition to model evaluation.

## Features

- Data loading and preprocessing from the MovieLens 20M dataset
- Exploratory Data Analysis (EDA) with visualizations
- Movie recommendation using:
  - User-based and item-based collaborative filtering
  - Matrix factorization approaches (e.g., SVD)
  - (Optionally) Content-based filtering using movie genres, tags, etc.
- Evaluation metrics such as RMSE, Precision@K, Recall@K

## Tech Stack and Libraries

- **Python 3.x**
- **Pandas**, **NumPy** (data handling)
- **Scikit-learn** (machine learning utilities)
- **Surprise** or **implicit** (for recommender system algorithms)
- **Matplotlib**, **Seaborn** (visualizations)
- **MovieLens ml-20m Dataset** (https://grouplens.org/datasets/movielens/20m/)

## Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ajaychaudhary8104/Movie_Recommendation_System_using_ml20.git
   cd Movie_Recommendation_System_using_ml20
   ```

2. **Install required packages:**
   Make sure you have Python 3.7+ installed.

   ```bash
   pip install -r requirements.txt
   ```

3. **Download the MovieLens 20M dataset:**
   Download from [here](https://grouplens.org/datasets/movielens/20m/) and extract the files into the `data/` directory in the root of the project.

## Data Preparation

- The project expects the MovieLens ml-20m dataset (CSV files: `ratings.csv`, `movies.csv`, etc.) inside the `data/` directory.
- Data preprocessing scripts will handle:
  - Parsing and cleaning the raw data.
  - Filtering users and movies to reduce sparsity.
  - Encoding categorical variables if content-based filtering is implemented.

## Models Implemented

- **User-based Collaborative Filtering:** Recommends movies based on similar users' preferences.
- **Item-based Collaborative Filtering:** Recommends movies similar to those the user has liked in the past.
- **Matrix Factorization (e.g., SVD):** Learns latent features for users and movies to predict ratings.
- **Content-Based Filtering:** (Optional) Recommends movies based on features like genre, keywords, etc.

## Results

- Visualizations and evaluation metrics are available in the `notebooks/` directory.
- Example results include:
  - Top-N recommendations for a user
  - RMSE, Precision@K and Recall@K on validation data

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with improvements, fixes, or suggestions.

1. Fork the repository.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Create a new Pull Request.

---

**Acknowledgments**

- [MovieLens Dataset - GroupLens Research](https://grouplens.org/datasets/movielens/)
- [Scikit-learn Documentation](https://scikit-learn.org)
- [Surprise Recommender System Library](http://surpriselib.com/)
