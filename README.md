# Credit Risk Prediction - Probability of Default (PD) Model

### Overview

This project focuses on building a binary classification model to predict whether a customer has good or bad credit based on financial indicators. Using features such as credit utilization, monthly income, and loan amount, the model estimates the probability of default (PD), helping financial institutions assess credit risk effectively.

### Dataset
The dataset contains financial and demographic information related to credit applicants. The key features used in this model include:

- Credit History – Previous loan repayment behavior.
- Purpose – The reason for applying for credit.
- Savings – Amount of savings available.
- Amount – Loan amount requested.
- Duration – Loan repayment period.

The target variable is Credit Risk (Good/Bad Credit), where 1 represents bad credit and 0 represents good credit.

### Methodology

1. Data Preprocessing
- Renamed German column names to English.
- Handled missing values through imputation or removal.
- Encoded categorical variables (nominal and ordinal).
- Standardized numerical features using StandardScaler.

2. Model Development
- Trained a Logistic Regression model for binary classification.
- Evaluated performance using AUC-ROC, precision, recall, and accuracy.
- Tuned the model to improve risk prediction.

3. Model Evaluation
- AUC-ROC: 0.793 (Good ability to distinguish between good/bad credit).
- Recall for bad credit: 89% (Effectively identifies defaulters).
- Recall for good credit: 45% (Some creditworthy customers misclassified).
- Overall accuracy: 76%.

### Results & Insights

- The model provides a reliable assessment of credit risk, but recall for good credit cases can be improved.
- Threshold tuning & feature engineering could further enhance precision.
- The approach can be extended with alternative models (Random Forest, XGBoost, or Neural Networks).

### Future Improvements

- Optimize classification threshold to reduce false positives.
- Try advanced ML models for better predictive power.
- Feature selection & engineering to improve accuracy.

### Source

![German Credit Data from Kaggle](https://www.kaggle.com/datasets/varunchawla30/german-credit-data)
