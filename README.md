# Credit-Score-Prediction-for-Paisabazaar
This project aims to develop a machine learning model that predicts a customer’s credit score—Good, Standard, or Poor—based on their financial behavior. It includes exploratory data analysis, model training, feature importance visualization, and deployment readiness.
# 📊 Credit Score Prediction for Paisabazaar

This project builds a machine learning model to predict a customer's credit score as **Good**, **Standard**, or **Poor** using financial and behavioral data. Built for the financial services platform Paisabazaar, the model supports automated, data-driven credit decisions to reduce risk and improve customer service.

---

## 📌 Project Objective

To predict credit scores based on:
- Income & salary
- Credit card usage
- Payment behavior
- Outstanding debt
- Occupation & credit mix

The goal is to enhance Paisabazaar’s credit assessment accuracy and streamline loan approval processes.

---

## 📁 Dataset

The dataset includes:
- `Annual_Income`
- `Monthly_Inhand_Salary`
- `Num_Credit_Card`
- `Outstanding_Debt`
- `Occupation`
- `Credit_Mix`
- `Payment_Behaviour`
- `Payment_of_Min_Amount`
- `Credit_Score` (target variable)

---

## 🔍 Exploratory Data Analysis (EDA)

Key patterns identified:
- Higher salary usually leads to better credit score.
- Credit behavior strongly impacts credit classification.
- Occupation and number of credit cards also show noticeable trends.

Visualizations include:
- Countplots of Credit Scores
- Cross-analysis of Occupation vs Credit Score
- Heatmaps and bar plots

---

## 🛠️ Data Preprocessing

Steps included:
- Handling missing values
- Dropping irrelevant columns
- Label encoding categorical features
- Normalization using `StandardScaler`

---

## 🤖 Models Trained

We trained and evaluated:
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier ✅ (Best Performer)

**Best Model: XGBoost**
- Accuracy: ~87%
- Balanced performance across classes

---

## 📊 Feature Importance

XGBoost identified:
- Monthly Inhand Salary
- Outstanding Debt
- Delay from Due Date
- Credit Utilization Ratio

These features contribute the most to the score prediction.

---

## 🧪 Prediction Function

A custom function allows real-time prediction from user input:

```python
def predict_credit_score(user_input_dict):
    # Data preprocessing steps...
    return predicted_score
