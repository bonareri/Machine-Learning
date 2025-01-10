# Customer Churn Prediction

## Overview
This project aims to predict customer churn using machine learning models and provide actionable insights to optimize retention strategies.

## Objectives
- Understand the key drivers of customer churn.
- Build a predictive model to identify at-risk customers.
- Develop recommendations to reduce churn and improve customer retention.

## Data Description
The dataset includes customer demographics, usage behavior, and payment information, featuring:\n
- **Demographics**: Age, Gender, Income.
- **Service Usage**: Monthly charges, tenure, contract type.
- **Payment Information**: Payment method, total charges.

## Key Steps
1. **Data Preprocessing**:
    - Handled missing values and outliers.
    - Scaled numerical features using MinMaxScaler.
    - Encoded categorical variables with Label Encoding.
    - Addressed class imbalance using SMOTE.

2. **Exploratory Data Analysis**:
    - Visualized churn distribution across demographics and service types.
    - Analyzed correlations between features and churn.

3. **Modeling**:
    - Tested multiple models: Logistic Regression, Random Forest, XGBoost.
    - Evaluated models using metrics such as accuracy, F1-score, and ROC-AUC.

4. **Feature Importance**:
    - Key predictors of churn include contract type, monthly charges, and payment method.

## Results
- Best model: [Insert Model Name] with an accuracy of [Value].
- ROC-AUC score: [Value].
- Insights:\n
  - Customers with short tenures and high monthly charges are more likely to churn.
  - Month-to-month contracts are a significant churn indicator.

## Recommendations
- Offer discounts for customers with month-to-month contracts.
- Incentivize long-term commitments through loyalty programs.
- Proactively address feedback from high-paying customers.

## Challenges and Limitations
- Class imbalance required oversampling techniques.
- Lack of real-time data limited the ability to deploy immediate actions.

## Future Work
- Incorporate sentiment analysis from customer feedback.
- Build a real-time prediction system.
