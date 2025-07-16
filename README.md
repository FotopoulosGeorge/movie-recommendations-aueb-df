# Movie Recommendation System

## Overview
A comprehensive movie recommendation system built for AUEB's AI/ML Data Factory course. This project implements both collaborative filtering and content-based filtering techniques to provide personalized movie recommendations using the MovieLens dataset and Wikipedia movie plots.

You can view the notebook here [![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg?logo=Jupyter)](https://nbviewer.org/github/FotopoulosGeorge/movie-recommendations-aueb-df/blob/main/Movie%20Recommendation%20System.ipynb)

## Features

### 1. **Genre Analysis**
- Identifies top-5 genres based on average movie ratings
- Provides insights into user preferences across different genres

### 2. **New User Onboarding**
- Suggests diverse, highly-rated movies to new users
- Balances popularity with genre diversity for cold-start scenarios

### 3. **Collaborative Filtering**
- Uses **Matrix Factorization (SVD)** for personalized recommendations
- Finds similar users and predicts ratings for unseen movies
- Handles new users by incorporating their ratings into the recommendation model

### 4. **Content-Based Filtering**
- Implements **TF-IDF vectorization** on movie plot descriptions
- Recommends movies with similar storylines and themes
- Provides explainable recommendations based on plot similarity

## Datasets
- **MovieLens 1M Dataset**: Contains 1M movie ratings from 6,000 users on 4,000 movies
- **Wikipedia Movie Plots**: 34,000+ movie plot summaries for content-based analysis

## Technical Implementation

### Machine Learning Techniques
- **Singular Value Decomposition (SVD)** for dimensionality reduction
- **TF-IDF (Term Frequency-Inverse Document Frequency)** for text analysis
- **Cosine Similarity** for measuring user and content similarity

### Data Processing
- User-item matrix construction and sparse matrix handling
- Text preprocessing and feature extraction
- Genre-based analysis and recommendation diversification

## Installation & Usage

### Requirements
```python
pandas==1.5.3
numpy==1.24.3
scikit-learn==1.3.0
matplotlib==3.7.1
seaborn==0.12.2
```

### Running the System
1. **Setup**: Ensure datasets are in the project directory
   - `movies.dat`
   - `ratings.dat` 
   - `tags.dat`
   - `wiki_movie_plots_deduped.csv`

2. **Execute**: Run the Jupyter notebook cells sequentially
3. **Customize**: Modify user ratings and parameters as needed

## Key Results

### Genre Insights
- **Film-Noir** has the highest average rating (4.01)
- **Documentary** and **War** genres also highly rated
- Action and Sci-Fi popular among users

### Recommendation Quality
- Matrix factorization successfully identifies user preferences
- Content-based filtering provides thematically similar recommendations
- System handles both warm and cold-start scenarios effectively

## Learning Outcomes
This project demonstrates:
- **Hybrid recommendation systems** combining multiple approaches
- **Real-world data preprocessing** and handling missing values
- **Scalable ML algorithms** for large-scale recommendation systems
- **Evaluation methodologies** for recommendation quality assessment

## Academic Context
**Course**: AI/ML Data Factory  
**Institution**: Athens University of Economics and Business (AUEB)  
**Focus**: Applied machine learning for recommendation systems

---

*This project showcases practical implementation of recommendation algorithms commonly used in industry applications like Netflix, Amazon, and Spotify.*
