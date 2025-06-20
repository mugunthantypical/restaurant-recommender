# Malaysian Restaurant Recommendation System

This project is a comprehensive restaurant recommendation system for Malaysian restaurants, built using collaborative and content-based filtering techniques. It leverages Google review data to provide personalized and relevant restaurant suggestions.

## Features

- **Data Preprocessing:** Cleans and processes raw Google review data for analysis.
- **Exploratory Data Analysis:** Visualizes rating distributions, top restaurants, and word clouds for insights.
- **Content-Based Filtering:** Recommends restaurants based on review text similarity using CountVectorizer and TF-IDF.
- **Collaborative Filtering:** Utilizes SVD and Surprise library for user-based recommendations.
- **Evaluation Metrics:** Calculates precision, recall, and F1-score for recommendation quality.

## Project Structure

```
GoogleReview_data_cleaned.csv
GoogleReview_KL.csv
restaurant-recommender-checkpoint.ipynb
.dist/
```

- **GoogleReview_data_cleaned.csv**: Cleaned review dataset for training and evaluation.
- **GoogleReview_KL.csv**: Additional review data for Kuala Lumpur.
- **restaurant-recommender-checkpoint.ipynb**: Main Jupyter notebook containing all code, analysis, and experiments.

## Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook
- Required libraries: `nltk`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `wordcloud`, `surprise`

### Installation

Install the required Python packages:

```sh
pip install nltk pandas numpy matplotlib scikit-learn wordcloud scikit-surprise
```

### Usage

1. **Open the notebook**  
   Launch Jupyter and open restaurant-recommender-checkpoint.ipynb.

2. **Run the cells**  
   Execute each cell in order to:
   - Import and preprocess the data
   - Visualize data insights
   - Build and evaluate recommendation models
   - Generate restaurant recommendations

3. **Modify parameters**  
   You can change the number of recommendations, user IDs, or target restaurants in the notebook cells to test different scenarios.

## Methods

- **Content-Based Filtering:**  
  Uses review text (after cleaning, tokenization, stemming) to compute similarity between restaurants and recommend similar ones.

- **Collaborative Filtering:**  
  Applies matrix factorization (SVD) to user-restaurant ratings to predict user preferences for unrated restaurants.

## Evaluation

The notebook includes functions to evaluate the recommendation system using precision, recall, and F1-score, comparing recommended restaurants to a ground truth set.

## Data

- The main dataset is GoogleReview_data_cleaned.csv, containing user reviews, ratings, restaurant names, and locations.
- Additional data for Kuala Lumpur is in GoogleReview_KL.csv.

## License

This project is for academic and research purposes.