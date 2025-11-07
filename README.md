# Rainfall-Prediction-Project

This project uses historical weather data to predict whether it will rain on the following day.  
The main goal was to prepare the data, train classification models, tune their parameters, and compare their performance.

The models evaluated were:
- Logistic Regression
- Random Forest Classifier

## Objective

Predict the target variable "RainTomorrow" (Yes/No) and evaluate which model performs better based on overall accuracy and true positive rate.

## Data Preparation

- Removed or imputed missing values
- Encoded categorical variables
- Normalized/standardized numerical features when necessary
- Split data into training and test sets
- Used pipeline and GridSearchCV to optimize model parameters

## Models

| Model                   | Notes |
|-------------------------|-------|
| Logistic Regression      | Used as a baseline model |
| Random Forest Classifier | Ensemble model with tree-based learning |

## Results

| Metric                 | Logistic Regression | Random Forest |
|-----------------------:|-------------------:|--------------:|
| Accuracy               | 83%                | 84%           |
| True Positive Rate     | 51%                | 50%           |
| Approx. Correct Predictions | ~1,255       | ~1,270        |

Interpretation:
- Random Forest achieved slightly higher accuracy and total correct predictions.
- Logistic Regression had a slightly higher true positive rate, meaning it identified rain events a bit better.
- The preferred model depends on whether the priority is overall accuracy or detecting rainy days.

## Possible Next Steps

- Experiment with boosted models (e.g., XGBoost, LightGBM)
- Try feature selection to reduce complexity
- Address class imbalance (rain events are less frequent) using SMOTE or class weights

## Tools and Libraries

- Python
- pandas
- numpy
- scikit-learn
- matplotlib / seaborn (optional visualizations)

## Dataset

Australian Bureau of Meteorology (public dataset).
