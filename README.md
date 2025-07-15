# 🏦 Bank Marketing Term Deposit Prediction

This project analyzes customer data to predict whether a client will subscribe to a term deposit using the Bank Marketing Dataset from the UCI repository.

## 📊 Dataset
- **Source**: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)
- **Records**: 45,211
- **Target**: `y` (1 = subscribed, 0 = not subscribed)

## 🔧 Key Steps
- Cleaned and encoded categorical data
- Created grouped features (age, balance, campaign)
- Visualized patterns (job type, age vs subscription, correlation matrix)
- Scaled numeric data for modeling

## 🤖 Models Used
- Logistic Regression
- Random Forest
- SVM
- XGBoost

**Best Models**: XGBoost, Random Forest  
**Top Metric**: ROC-AUC up to ~0.91

## 📁 Files
- `BankMarketingCSV.csv` – Dataset  
- `bank_marketing_analysis.ipynb` – Full Colab notebook  
- `README.md` – Project overview

## 🔗 Colab Notebook
👉 [Open in Colab](https://colab.research.google.com/drive/1-6GKQyyvsAw9z7lm8NXTXsQfTU3sCv84?usp=sharing)
