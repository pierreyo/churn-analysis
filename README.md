# Churn Prediction for Bank Customers

# Project Overview

This project focuses on predicting customer churn in a banking dataset using various machine learning models. We analyze customer features, explore different modeling approaches, and compare performance with and without Synthetic Minority Over-sampling Technique (SMOTE).

# Dataset

The dataset consists of customer information such as:

Numerical Features: Credit Score, Age, Tenure, Balance, Estimated Salary, etc.

Categorical Features: Geography, Gender, Number of Products, etc.

Target Variable: Exited (1 = Churn, 0 = Retained)

Exploratory Data Analysis (EDA)

1. Initial Analysis

Checked for missing values

Performed basic statistical summaries

2. Numerical Feature Visualization

Distribution plots

Correlation heatmaps

3. Categorical Feature Visualization

Count plots

Churn distribution across categories

Machine Learning Models

1. Models Used

We trained and compared the following models:

Logistic Regression

Decision Tree

Random Forest with RandomizedSearchCV

XGBoost

2. Models with and without SMOTE

We tested models with and without SMOTE to balance the dataset.

Key Findings:

Random Forest without SMOTE performed best, achieving 86% accuracy.

Models without SMOTE had better accuracy but struggled with lower true positive rates (Churn predicted correctly).

SMOTE improved recall (capturing more churn cases) but reduced overall accuracy.

Best Model Performance (Random Forest without SMOTE)

Accuracy: 86%

Confusion Matrix: High precision but lower recall for churn cases

Feature Importance (SHAP Analysis):

Age and Number of Products were key predictors

Balance and Credit Score also had strong influence

Conclusion

Random Forest without SMOTE is the best model, striking a balance between accuracy and churn detection.

Future Work: Consider additional feature engineering, ensemble learning, or cost-sensitive learning to improve true positive detection.
