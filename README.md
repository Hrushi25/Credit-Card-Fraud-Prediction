# 💳 Credit Card Fraud Detection System

An interactive fraud detection system that uses machine learning to predict the likelihood of a transaction being fraudulent. The system includes both a backend ML model and a frontend dashboard for visual analysis and transaction simulation.

![App UI](screenshots/credit-fraud-ui.png)

---

## 📌 Overview

This project analyzes credit card transaction data to detect fraudulent activity using various classification algorithms like Logistic Regression, Random Forest, and XGBoost. It features:

- A clean and interactive dashboard
- Real-time transaction scoring
- Feature importance and risk factors
- Model evaluation via AUC, confusion matrix, and fraud rate analysis

---

## ⚙️ Technologies Used

- **Python** (Pandas, Scikit-learn, XGBoost)
- **Streamlit** (or custom dashboard framework)
- **Matplotlib / Seaborn / Plotly**
- **Jupyter Notebook** for analysis
- **HTML/CSS** (if applicable for dashboard visuals)

---

## 📊 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Records:** 284,807 transactions
- **Fraud Ratio:** 0.17%

---

## 🧠 Features

### ✅ Fraud Prediction Interface

Users can input transaction info:
- Amount
- Hour of transaction
- Distance between customer and merchant
- City population, time, and date

Based on this, the system returns:
- ✅ **Risk Score**  
- ✅ **Transaction Classification**
- ✅ **Risk Factor Indicators**
- ✅ **Feature Importance Breakdown**

![Prediction UI](screenshots/credit-fraud-dashboard.png)

---

### 📈 Model Evaluation Dashboard

Includes performance comparison of different ML models:
- Logistic Regression
- Random Forest
- XGBoost

Key visualizations:
- Class imbalance visualization
- Feature importance chart
- Fraud rate vs hour of day
- Confusion matrix (TP, FP, TN, FN)

![Model Comparison](screenshots/confusion-matrix.png)

---

## 🧪 Modeling Workflow

1. **Data Cleaning**
   - Drop duplicates, handle missing values
2. **EDA & Visualization**
   - Class distribution, correlations, time-based fraud analysis
3. **Feature Engineering**
   - Custom fields: transaction hour, day, distance
4. **Handling Imbalance**
   - Random under/oversampling, SMOTE
5. **Model Training & Tuning**
   - Cross-validation, ROC-AUC scoring
6. **Evaluation**
   - Confusion matrix, recall, precision

---

## 📌 Key Insights

- Dataset is **highly imbalanced** — only ~0.39% of transactions are fraud.
- **Random Forest** has the best AUC score (0.67), followed by XGBoost.
- **Amount and distance** are most influential features.
- **Most frauds occur between midnight and 5 AM**.
- High accuracy is misleading — focus on **recall for fraud detection**.
- Best model caught ~35% of actual frauds.

---

