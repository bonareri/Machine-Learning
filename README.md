# Customer Churn Prediction

## Overview
This project aims to predict customer churn using machine learning models and provide actionable insights to optimize retention strategies.

## Objectives
- Understand the key drivers of customer churn.
- Build a predictive model to identify at-risk customers.
- Develop recommendations to reduce churn and improve customer retention.

## Data Description
The dataset includes customer demographics, usage behavior, and payment information, featuring:\n
- **customerID**: A unique identifier for each customer in the dataset.
- **gender**: The gender of the customer (e.g., "Male" or "Female").
- **SeniorCitizen**: Indicates whether the customer is a senior citizen (1 = Yes, 0 = No).
- **Partner**: Indicates whether the customer has a partner (e.g., "Yes" or "No").
- **Dependents**: Indicates whether the customer has dependents (e.g., "Yes" or "No").
- **tenure**: The number of months the customer has stayed with the company.
- **PhoneService**: Indicates whether the customer has phone service (e.g., "Yes" or "No").
- **MultipleLines**: Indicates whether the customer has multiple phone lines (e.g., "Yes", "No", or "No phone service").
- **InternetService**: The type of internet service the customer has (e.g., "DSL", "Fiber optic", "No").
- **OnlineSecurity**: Indicates whether the customer has online security service (e.g., "Yes", "No", or "No internet service").
- **OnlineBackup**: Indicates whether the customer has online backup service (e.g., "Yes", "No", or "No internet service").
- **DeviceProtection**: Indicates whether the customer has device protection service (e.g., "Yes", "No", or "No internet service").
- **TechSupport**: Indicates whether the customer has technical support service (e.g., "Yes", "No", or "No internet service").
- **StreamingTV**: Indicates whether the customer has streaming TV service (e.g., "Yes", "No", or "No internet service").
- **StreamingMovies**: Indicates whether the customer has streaming movie service (e.g., "Yes", "No", or "No internet service").
- **Contract**: The type of contract the customer has (e.g., "Month-to-month", "One year", "Two year").
- **PaperlessBilling**: Indicates whether the customer uses paperless billing (e.g., "Yes" or "No").
- **PaymentMethod**: The payment method used by the customer (e.g., "Electronic check", "Mailed check", "Bank transfer (automatic)", "Credit card (automatic)").
- **MonthlyCharges**: The amount charged to the customer monthly (float).
- **TotalCharges**: The total amount charged to the customer over the tenure period (recorded as an object, though it likely represents a numeric value).
- **Churn**: Indicates whether the customer has churned (i.e., stopped using the service; "Yes" = churned, "No" = retained).

## Key Steps
1. **Data Preprocessing**:
    - Scaled numerical features using MinMaxScaler.
    - Encoded categorical variables with Label Encoding.
    - Addressed class imbalance using SMOTE.

2. **Exploratory Data Analysis**:
    - Visualized churn distribution across demographics and service types.
    - 
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
