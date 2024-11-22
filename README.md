# House Prices Prediction Project

## Overview
This project aims to predict house prices using the **Kaggle House Prices** dataset. The goal is to develop a model that accurately estimates the sale prices of homes based on various features, such as house attributes, neighborhood, and construction details. The project includes data exploration, feature engineering, model training, hyperparameter optimization, and evaluation.

## Dataset
The dataset used in this project comes from the **Kaggle House Prices - Advanced Regression Techniques** competition.
The dataset can be downloaded from [Kaggle House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).

## Project Workflow
### 1. Data Exploration
- Analyzing the distribution of features and target values.
- Visualizing correlations between features.
- Identifying and handling missing values, outliers, and NaN entries.

### 2. Data Preprocessing
- **Handling Missing Values**: 
  - Numerical features are imputed using the mean.
  - Categorical features are imputed using the most frequent value.
- **Encoding Categorical Variables**: Using one-hot encoding to convert categorical variables to numerical format.
- **Feature Scaling**: Scaling numerical features to standardize their ranges.

### 3. Feature Engineering

### 4. Model Training and Evaluation
Various machine learning models are trained and evaluated using cross-validation:
- **Models Used**:
  - ElasticNet
  - Random Forest Regressor
  - Histogram-Based Gradient Boosting (HistGradientBoosting)
- **Hyperparameter Optimization**: Performed using Optuna to find the best parameters for each model.
- **Evaluation Metric**: Mean Absolute Percentage Error (MAPE) is used to evaluate model performance.
- **Final Model**: The best model is selected based on cross-validation scores and trained on the full training dataset.

### 5. Predictions and Submission
- Predictions are made on the test dataset after training the final model.
- Results are saved in the `submission.csv` file for submission to Kaggle.
