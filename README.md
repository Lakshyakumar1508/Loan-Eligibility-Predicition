# 🏦 Loan Eligibility Predictor

This project predicts whether a loan applicant should be **approved or rejected** using classification models trained on personal, financial, and credit-related features. It's built using **Logistic Regression** and **Random Forest**, and includes full preprocessing and evaluation.

---

## 📌 Problem Statement

Financial institutions want to reduce loan default risks by assessing whether an applicant is eligible for a loan. This project uses machine learning models to make those predictions based on features such as:

- Home ownership
- Income
- Credit history
- Employment length
- Loan amount and purpose

---

## 🧾 Dataset Overview

The dataset includes the following features:

| Column                        | Description                                      |
|------------------------------|--------------------------------------------------|
| `person_home_ownership`      | RENT, OWN, MORTGAGE, etc.                        |
| `loan_intent`                | Purpose of loan: PERSONAL, MEDICAL, EDUCATION   |
| `loan_grade`                 | Loan grade (A–G)                                 |
| `cb_person_default_on_file` | Past default status (Y/N)                        |
| `person_income`              | Applicant’s income                               |
| `person_age`                 | Age of applicant                                 |
| `person_emp_length`          | Employment length in months                      |
| `loan_amnt`                  | Loan amount requested                            |
| `loan_int_rate`              | Interest rate on the loan                        |
| `cb_person_cred_hist_length`| Credit history length (years)                    |
| `loan_percent_income`        | Loan amount as % of income                       |
| `loan_status`                | **Target**: 1 = Approved, 0 = Rejected           |

---

## ⚙️ Technologies Used

- Python 🐍
- pandas, NumPy
- scikit-learn (LogisticRegression, RandomForest)
- Matplotlib & Seaborn (for plots)
- Jupyter Notebook or Python script

---

## 📊 Model Workflow

1. **Load Dataset**
2. **Handle Missing Values**
3. **Encode Categorical Variables**
4. **Feature Scaling**
5. **Train-Test Split**
6. **Train Models:**
   - Random Forest Classifier
7. **Evaluate:**
   - Confusion Matrix
   - Classification Report
   - ROC Curve & AUC
8. **Predict for New Applicant**

----
Random Forest - Classification Report
              precision    recall  f1-score   support

           0       0.92      0.99      0.96      5072
           1       0.96      0.71      0.82      1445

    accuracy                           0.93      6517
   macro avg       0.94      0.85      0.89      6517
weighted avg       0.93      0.93      0.93      6517

