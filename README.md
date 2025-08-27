# Fraud_Detection
This repository contains my solution for the Fraud Detection Case Study provided as part of Accredian’s screening round. The goal of the project is to proactively detect fraudulent transactions using machine learning techniques and provide business insights for prevention.

# Repository Contents
Fraud_Detection.ipynb → Jupyter Notebook with end-to-end code (data cleaning, preprocessing, model training, evaluation, insights).
Data Dictionary.txt → Metadata file describing each feature in the dataset.
Fraud.csv → Dataset file (not included here due to size/privacy; upload separately).
README.md → Project overview and usage instructions.

# Approach
1. Data Cleaning & Preprocessing
Removed irrelevant identifiers (nameOrig, nameDest).
Handled missing values (median imputation).
Encoded categorical variable type using one-hot encoding.
Addressed outliers using IQR filtering.

2. Imbalance Handling
Applied SMOTE to balance fraudulent vs. non-fraudulent cases.
Also set class_weight=balanced for classifiers.

3. Model Training
Logistic Regression (baseline).
Random Forest (interpretable, feature importance).
XGBoost (best-performing gradient boosting model).

4. Evaluation Metrics
Classification Report (Precision, Recall, F1-Score).
Confusion Matrix.
ROC-AUC Curve.
(Optional) Precision-Recall Curve (highly useful for imbalanced datasets).

5. Key Insights
High transaction amounts and unusual transaction types strongly indicate fraud.
Transactions from new accounts or unusual devices/IPs show higher fraud probability.
Recommended fraud prevention: real-time monitoring, multi-factor authentication, periodic model retraining, and anomaly detection systems.

# Tools & Libraries
Python (Pandas, NumPy, Matplotlib, Seaborn)
Scikit-learn
XGBoost
Imbalanced-learn (SMOTE)

# Dataset
Due to file size limits, the dataset is not stored in this repository.
You can download it here: https://drive.usercontent.google.com/download?id=1VNpyNkGxHdskfdTNRSjjyNa5qC9u0JyV&export=download&authuser=0
