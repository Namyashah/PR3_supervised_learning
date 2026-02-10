![Screenshot](images/Screenshot%202026-02-09%20201900.png)
# 💳 Risk Alert Classifier

An end-to-end Machine Learning project to predict whether a customer is
high risk or low risk using financial, behavioral, and
transaction data.

The goal is to help financial institutions minimize defaults and make
smarter lending decisions.

------------------------------------------------------------------------

## 🚀 Project Highlights

✅ Data Cleaning & Missing Value Treatment\
✅ Feature Engineering from transaction dates\
✅ Encoding & Scaling using ColumnTransformer\
✅ Handling Imbalanced Data (UnderSampling, SMOTE, ADASYN)\
✅ Logistic Regression, Decision Tree & Random Forest\
✅ Hyperparameter tuning with GridSearchCV & RandomizedSearchCV\
✅ Overfitting & Generalization analysis\
✅ ROC-AUC evaluation\
✅ Business interpretation of errors\

------------------------------------------------------------------------

## 📂 Dataset Overview

The dataset includes:

-   Demographics (age, gender, region)
-   Financials (income, debt, credit score)
-   Behavior (missed payments, utilization ratio)
-   Activity patterns (transactions, complaints)
-   Target → risk_status (0 = safe, 1 = risky)

------------------------------------------------------------------------

## 🧹 Data Preprocessing

-   Removed unnecessary identifiers
-   Converted dates into useful numerical features
-   One-Hot Encoded categorical variables
-   Standardized numerical variables
-   Built preprocessing into pipelines to avoid leakage

------------------------------------------------------------------------

## ⚖️ Handling Class Imbalance

Since high-risk customers were fewer:

🔹 Random Under Sampling\
🔹 SMOTE\
🔹 ADASYN\
👉 This improved recall and F1 score for risky customers.

------------------------------------------------------------------------

## 🤖 Models Implemented

-   Logistic Regression
-   Decision Tree
-   Random Forest

------------------------------------------------------------------------

## 🎯 Model Tuning

To improve performance and reduce overfitting:

✔ GridSearchCV → Decision Tree\
✔ RandomizedSearchCV → Random Forest

------------------------------------------------------------------------

## 📊 Evaluation Metrics

Because accuracy can be misleading in imbalance, we focused on:

✅ Recall (minority class)\
✅ F1 Score\
✅ ROC-AUC

------------------------------------------------------------------------

## 📈 ROC--AUC

Used probability predictions to measure how well the model separates
risky vs safe customers across thresholds.

Higher AUC = better ranking ability.

------------------------------------------------------------------------

## 💼 Business Understanding of Errors

🔴 False Negative → Risky customer predicted safe → financial loss\
🟡 False Positive → Safe customer flagged risky → customer inconvenience

👉 Reducing false negatives is critical.

------------------------------------------------------------------------

## 🛠 Tech Stack

Python 🐍\
Pandas & NumPy\
Scikit-Learn\
Imbalanced-Learn\
Matplotlib / Seaborn

------------------------------------------------------------------------