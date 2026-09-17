# customer_churn_prediction
this is the project in which we predict whether the customer will churn or not and we have made comparisons by using ml model
# Telco Customer Churn Prediction

A Machine Learning project that predicts whether a telecom customer is likely to churn based on their demographic, service, contract, and billing information.

The project uses **Logistic Regression** for classification and provides a **FastAPI REST API** that allows users to send customer information and receive a churn prediction with probability.

---

## Project Overview

Customer churn is an important problem for telecom companies. Being able to identify customers who are likely to leave can help businesses take action and improve customer retention.

In this project, I:

- Loaded and explored a Telco Customer Churn dataset
- Cleaned and prepared the data
- Performed Exploratory Data Analysis (EDA)
- Analyzed factors related to customer churn
- Applied numerical and categorical preprocessing
- Built a Logistic Regression classification model
- Evaluated the model
- Saved the trained model using Joblib
- Built a FastAPI application
- Created a `/predict` API endpoint
- Tested the API using FastAPI Swagger UI

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- FastAPI
- Uvicorn
- Jupyter Notebook

---

## Dataset

The project uses a Telco Customer Churn dataset containing information about telecom customers.

Some of the features include:

- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Phone Service
- Multiple Lines
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming TV
- Streaming Movies
- Contract
- Paperless Billing
- Payment Method
- Monthly Charges
- Total Charges

The target variable is:

**Churn**

- `Yes` → Customer churned
- `No` → Customer did not churn

---

## Exploratory Data Analysis

Several analyses and visualizations were performed to understand customer churn.

The project examined relationships between churn and:

- Contract type
- Tenure
- Monthly Charges
- Internet Service
- Payment Method
- Tech Support
- Other customer and service characteristics

These visualizations helped identify patterns and factors associated with customer churn.

---

## Machine Learning Model

### Logistic Regression

Logistic Regression was used as the classification algorithm because the target variable contains two possible outcomes:

- Churn
- No Churn

The project uses a Scikit-learn pipeline containing:

1. Data preprocessing
2. Numerical feature scaling using `StandardScaler`
3. Categorical feature encoding using `OneHotEncoder`
4. Logistic Regression classifier

The complete preprocessing and prediction pipeline was saved using Joblib.

---

## Model File

The trained model is saved as:

```text
customer_churn_model.joblib
