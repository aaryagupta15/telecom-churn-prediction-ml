# Telecom Customer Churn Prediction

This repository presents a machine learning-based approach to predict customer churn for a telecom company. The goal is to identify high-risk customers and enable the business to take preventive retention actions.

## 🔍 Project Overview

Customer churn is a critical challenge for telecom companies, directly affecting revenue and customer acquisition cost. This project focuses on building a predictive model using customer demographic, account, and usage data to classify whether a customer is likely to churn.

## 📁 Dataset

- **Source**: [Kaggle - Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Rows**: 7,043  
- **Target Variable**: `Churn` (Yes/No)  
- **Key Features**:  
  - Contract Type  
  - Monthly & Total Charges  
  - Tenure  
  - Internet & Streaming Services  
  - Payment Method  
  - Senior Citizen, Dependents, and Partner Status

## 📊 Exploratory Data Analysis (EDA)

Performed comprehensive EDA using `seaborn`, `matplotlib`, and `plotly`:
- Checked data types and handled missing values (e.g., `TotalCharges` conversion).
- Visualized churn rate by features like gender, tenure, and internet service.
- Observed that shorter tenure and fiber-optic service strongly correlated with higher churn.

## 🧹 Data Preprocessing

- Encoded categorical variables using one-hot encoding.
- Scaled numerical features with StandardScaler.
- Removed irrelevant columns like `customerID`.
- Split the data into training, validation, and test sets using stratified sampling.

## 🤖 Model Training & Tuning

- Used `LazyPredict` to benchmark multiple classification models.
- Selected **XGBoost** for final training based on superior accuracy and F1-score.
- Performed **GridSearchCV** for hyperparameter tuning.
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC

## 🧠 Model Interpretation

- Applied **SHAP** to understand feature importance and improve explainability.
- Top predictive features included:
  - Monthly Charges
  - Tenure
  - Contract Type (Month-to-Month)
  - Internet Service Type

## 📌 Business Use Case

Created a **Churn Risk Probability Table** that ranks customers based on churn likelihood. This can help marketing and support teams prioritize customers for retention campaigns.

## 📈 Model Results

| Metric      | Score     |
|-------------|-----------|
| Accuracy    | 81.9%     |
| Precision   | 67.1%     |
| Recall      | 52.0%     |
| F1 Score    | 58.6%     |
| ROC-AUC     | 0.816     |

## 🚀 Tech Stack

- Python (Pandas, NumPy, Scikit-learn, XGBoost, SHAP, Matplotlib, Seaborn, Plotly)

## 📬 Contact

For queries or collaboration opportunities, feel free to connect:

**Aarya Gupta**  
📧 g.aarya1504@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aarya-gupta-26486a22a) | [GitHub](https://github.com/aaryagupta15)

