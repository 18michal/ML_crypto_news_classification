# Cryptocurrency Sentiment Analysis and Bitcoin Price Correlation

## Project Overview
This project analyzes the sentiment of cryptocurrency news articles and explores the correlation between sentiment and Bitcoin price changes over time.

### Dataset
1. **Crypto News Dataset**
   - Source: [Kaggle - Crypto News Dataset](https://www.kaggle.com/datasets/oliviervha/crypto-news/data)
   - Description: Contains 31,037 news articles (2021-10-12 to 2023-12-19).

2. **Bitcoin Historical Data**
   - Source: [Kaggle - Bitcoin Historical Data](https://www.kaggle.com/datasets/armanzhalgasbayev/bitcoin-historical-data-2021-2023)
   - Description: Includes Bitcoin price, percentage changes, and related market data.

## Goals
1. Build a classification model to predict news sentiment as Positive, Neutral, or Negative.
2. Explore the relationship between sentiment trends and Bitcoin price changes.

---

## Key Steps

### 1. Data Preprocessing and EDA
### 2. Model Training
- **Features**: Combined `title` and `text` fields.
- **Vectorization**: Applied TF-IDF (Term Frequency-Inverse Document Frequency).
- **Classifier**: Logistic Regression with hyperparameter tuning via GridSearchCV.
- **Performance**:
  - Accuracy: **73%**
  - Best parameters: `C=10`, `penalty=l1`, `solver=liblinear`.

### 3. Sentiment and Price Analysis
- Correlation Heatmap: Grouped by Monthly Data.
- Scatter Plot: Visualized Bitcoin price over time, color-coded by dominant sentiment.
