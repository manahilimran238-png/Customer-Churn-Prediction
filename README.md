# 📊 Customer Churn Prediction System

A machine learning project that predicts whether a customer is likely to churn or continue using a service. The project includes data preprocessing, exploratory data analysis, multiple classification models, feature importance analysis, and an interactive Streamlit application.

## 🎯 Project Objective

Customer churn can negatively affect business revenue and customer retention. This project analyzes customer demographic, service, contract, and billing information to identify customers who are more likely to leave a service.

The system compares multiple machine learning models and provides an interactive interface for making churn predictions.

## 📂 Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information such as:

- Customer demographics
- Tenure
- Contract type
- Internet service
- Online security and support services
- Payment method
- Monthly charges
- Total charges
- Churn status

After cleaning, the dataset contained **7,032 customer records** and **21 columns**.

## 🔄 Project Workflow

1. Data Collection
2. Data Cleaning
3. Exploratory Data Analysis
4. Feature Engineering
5. Data Preprocessing
6. Train-Test Split
7. Model Training
8. Model Evaluation
9. Feature Importance Analysis
10. Customer Churn Prediction
11. Streamlit Application

## 📊 Exploratory Data Analysis

The analysis investigated:

- Churn distribution
- Monthly charges vs churn
- Customer tenure vs churn
- Contract type and churn
- Feature correlations with churn

Some important findings included:

- Customers who churned had higher average monthly charges.
- Churned customers had considerably lower average tenure.
- Month-to-month contracts had substantially higher churn than one-year and two-year contracts.
- Fiber-optic internet service and electronic check payment showed notable relationships with churn.

## 🤖 Machine Learning Models

Three classification models were trained and evaluated:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

### Model Performance

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 80.53% | 65.15% | 57.49% | 61.08% |
| Decision Tree | 77.83% | 58.07% | 59.63% | 58.84% |
| Random Forest | 77.26% | 55.36% | 74.60% | 63.55% |

Random Forest achieved the highest **Recall (74.60%)** and **F1 Score (63.55%)**, making it useful for identifying customers who may be at risk of churn.

Logistic Regression achieved the highest overall **Accuracy (80.53%)** and **Precision (65.15%)**.

## 🔍 Important Features

Random Forest feature importance identified several influential features:

- Tenure
- Total Charges
- Monthly Charges
- Contract Type
- Internet Service
- Payment Method
- Online Security
- Technical Support

The most important feature was **tenure**, followed by **Total Charges** and **Monthly Charges**.

## 🖥️ Streamlit Application

The project includes an interactive Streamlit application where users can enter customer information and receive a churn prediction.

The application displays:

- Customer information form
- Churn prediction
- Churn probability
- Stay/Churn result

### Example Prediction

A high-risk customer profile produced:

**Customer is likely to churn**

**Churn Probability: 86.58%**

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Streamlit
- Joblib
- Jupyter Notebook / Google Colab

## 📁 Project Structure

```text
Customer-Churn-Prediction/
│
├── Customer_Churn_Prediction.ipynb
├── app.py
├── customer_churn_model.pkl
├── requirements.txt
└── README.md
