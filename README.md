 Bank Marketing Term Deposit Prediction:
This project uses the Bank Marketing Dataset from the UCI Machine Learning Repository to predict whether a client will subscribe to a term deposit (y = 1). It explores relationships between customer demographics, campaign features, and past interactions with the bank using exploratory data analysis and machine learning models.

📊 Dataset
Source: UCI Bank Marketing Dataset

Records: 45,211

Features: Age, job, marital status, education, default status, balance, housing, loan, contact type, month, campaign, previous outcomes, etc.

Target: y — whether the client subscribed to a term deposit (1 = yes, 0 = no)

🔧 Key Steps
Data Preprocessing
Removed duplicates

Mapped binary categorical variables (yes/no) to 1/0

One-hot encoded categorical variables (job, marital, education, contact, month, poutcome)

Created custom categorical groupings:

age_group: Binned age into 5 groups

balance_category: Negative, Low, Medium, High

campaign_intensity: Binned campaign frequency

Feature Engineering
One-hot encoding of new grouped features

Standardized numerical features using StandardScaler

Data Visualization
Distribution of term deposit subscriptions

Boxplot of age by subscription status

Subscription rate by job type

Correlation heatmap

🤖 Modeling
Algorithms Used
Logistic Regression

Random Forest

Support Vector Machine (SVM)

XGBoost Classifier

Evaluation Metrics
Classification Report (Precision, Recall, F1-score)

Confusion Matrix

ROC-AUC Score

Model	ROC-AUC Score
Logistic Regression	~0.77
Random Forest	~0.90
SVM	~0.88
XGBoost	~0.91

🧠 Results
Best Models: XGBoost and Random Forest

Top Features: Contact type, month of campaign, job type, campaign frequency

Insights: Clients contacted via cellular in months like May and August had higher subscription rates.

📁 Project Structure
bash
Copy
Edit
bank_marketing_prediction/
│
├── BankMarketingCSV.csv           # Dataset
├── bank_marketing_analysis.ipynb  # Colab notebook with full pipeline
├── README.md                      # Project overview (this file)
🔗 Colab Notebook
👉 View Full Project in Google Colab
