# telco_customer-churn-prediction
End-to-end churn prediction project using Random Forest and risk scoring
# Telco Customer Churn Prediction

## Problem
Customer churn is a critical business problem in the telecom industry.
This project aims to identify customers who are likely to leave the service
and rank them based on churn risk for targeted retention actions.

## Dataset
- Telco Customer Churn Dataset (Kaggle)
- 7,043 customers, 21 features

## Preprocessing
- Removed customerID to prevent data leakage
- Converted TotalCharges to numeric
- Applied one-hot encoding for categorical variables
- Handled class imbalance using class_weight

## Model
- Random Forest Classifier
- Hyperparameters tuned (n_estimators, max_depth)
- Class imbalance handled via class_weight

## Evaluation
- Accuracy: ~0.79
- Recall (Churn = Yes): ~0.77
- Confusion Matrix and Classification Report analyzed

## Churn Risk Scoring
- Predicted churn probabilities using predict_proba
- Ranked customers by churn risk
- Identified high-risk customers for proactive retention

## Business Impact
- High-risk customers can be targeted with retention offers
- Reduces revenue loss by prioritizing recall over precision

## Technologies
- Python
- Pandas
- Scikit-learn
- Google Colab
