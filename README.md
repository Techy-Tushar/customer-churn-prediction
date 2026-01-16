# 📊 Customer Churn Prediction (Machine Learning)

## 🧩 Overview
Customer churn is a critical challenge for banks, as retaining existing customers is more cost-effective than acquiring new ones.  
This project builds an **end-to-end machine learning solution** to predict customer churn and identify the key factors driving customer attrition, enabling proactive retention strategies.

---

## 🎯 Objectives
- 🔮 Predict whether a customer is likely to churn  
- 🔍 Identify the most important churn drivers  
- ⚙️ Compare multiple classification models  
- ✅ Select a robust and business-oriented final model  

---

## 📂 Dataset
- Customer demographic, financial, and engagement data  
- 🎯 **Target Variable:** `Exited`  
  - `1` → Churned  
  - `0` → Retained  

Features include age, geography, credit score, balance, number of products, activity status, card details, and more.

> ⚠️ Complaint and satisfaction-related features were carefully handled to avoid **data leakage**.

---

## 🧪 Project Workflow

### 📌 Data Understanding & Preprocessing
- Dataset inspection  
- Removal of irrelevant columns  
- Column renaming and one-hot encoding  

### 📊 Exploratory Data Analysis (EDA)
- Target variable distribution  
- Categorical vs churn analysis  
- Numerical vs churn analysis  
- Correlation analysis  

### 🧠 Modeling Strategy
- Train–test split with stratification  
- Metrics prioritized: **Recall** and **ROC-AUC**  

### 🤖 Models Evaluated
- Logistic Regression (Baseline)  
- Logistic Regression (Class-Weighted)  
- Random Forest  
- XGBoost  

### 📈 Model Comparison
- Compared using **Accuracy**, **Churn Recall**, and **ROC-AUC**  

### 🔧 Hyperparameter Tuning
- GridSearchCV applied to XGBoost  
- Optimized for **ROC-AUC**  

### 🏆 Final Model Selection
- Tuned **XGBoost** selected as the final model  

### 🔎 Feature Importance & Business Insights
- Identified key churn drivers  
- Translated insights into actionable recommendations  

---

## 📌 Key Results

| Metric | Tuned XGBoost |
|------|---------------|
| 🎯 Accuracy | ~80% |
| 🔁 Churn Recall | ~78% |
| 📐 ROC-AUC | ~0.88 |

---

## 🔑 Key Churn Drivers
- 👤 Age  
- 📦 Number of Products  
- ⚡ Customer Activity Status  
- 🌍 Geography  
- 💰 Account Balance  

---

## 💡 Business Recommendations
- 🎯 Focus retention efforts on high-risk age segments  
- 📈 Increase product adoption through cross-selling  
- 🤝 Improve engagement for inactive customers  
- 🗺️ Apply region-specific churn strategies  
- 🎁 Offer targeted financial incentives to low-balance customers  

---

## 🛠️ Technologies Used
- 🐍 Python  
- 📊 Pandas, NumPy  
- 📉 Matplotlib, Seaborn  
- 🤖 Scikit-learn  
- 🚀 XGBoost  

---

## ⚠️ Limitations & Future Work
- Assumes future churn patterns are similar to historical data  
- ⏱️ Time-series behavioral data could further improve performance  
- 🎚️ Threshold optimization and deployment are potential next steps  

---

## 👤 Author
**Tushar Rathod**
