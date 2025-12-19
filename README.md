# 🏦 Home Loan Repayment Prediction — Joana Coyle

## Overview
End-to-end **credit risk classification** project predicting whether a loan applicant will **repay or default**, using structured financial and demographic data.  
Built to demonstrate **production-ready ML practices**, not just model accuracy.

---

## Dataset
- Home loan application records  
- **Target:** Loan Repayment Status (Repaid / Default)  
- Features include income, loan amount, credit history, employment status, and demographics  
- Dataset is **highly imbalanced** (defaults underrepresented)

---

## Workflow (High Level)
- Data cleaning & validation (missing values, duplicates)
- Exploratory data analysis to identify risk drivers
- Outlier treatment using **IQR filtering + winsorization**
- Feature encoding and scaling
- Dimensionality reduction with **PCA**
- Class imbalance handled with **SMOTE (training data only)**

---

## Modeling
- Logistic Regression (baseline)
- Neural Network (TensorFlow / Keras)
- Threshold tuning to improve default detection
- Evaluation with:
  - Precision / Recall
  - ROC–AUC
  - Confusion Matrix

---

## Key Insights
- **Credit history** is the strongest predictor of repayment
- Income alone is not sufficient for risk assessment
- Class imbalance strongly impacts baseline performance
- Threshold tuning improves identification of high-risk applicants

---

## Notes on Design Choices
- **Outliers:** Extreme financial values were removed using IQR; remaining high-variance values were capped with winsorization to improve model stability without excessive data loss  
- **PCA:** High number of components retained due to one-hot encoded feature space  
- **Warnings:** Some pandas/seaborn `FutureWarning`s may appear in GitHub preview; they do not affect results


