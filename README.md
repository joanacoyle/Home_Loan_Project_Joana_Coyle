# Home Loan Repayment Prediction — Joana Coyle

## Overview
Credit risk analysis project using **exploratory data analysis (EDA) and machine learning** to predict whether a loan applicant will repay or default, supporting data-driven lending decisions.

---

## Dataset
- Home loan application records  
- **Binary target:** Loan Repayment Status (Repaid / Default)  
- **Key features include:**  
  - Applicant income  
  - Loan amount  
  - Credit history  
  - Employment status  
  - Property area  
  - Demographic and financial attributes  

> Note: The dataset contains class imbalance, which was addressed during preprocessing.

---

## Workflow

### Data Wrangling & Validation
- Checked and handled missing values  
- Removed duplicate records  
- Preserved an untouched copy of the original dataset  
- Encoded categorical variables  
- Scaled numerical features for model stability  

### Exploratory Data Analysis (EDA)
- Identified skewed distributions in income and loan amount  
- Confirmed **credit history** as a dominant factor in repayment outcomes  
- Analyzed repayment behavior by:
  - Income level  
  - Loan amount  
  - Employment status  
  - Property area  
- Verified class imbalance in the target variable  

### Feature Engineering
- Applied feature scaling using **StandardScaler / MinMaxScaler**  
- Reduced dimensionality using **PCA**  
- Addressed class imbalance using **SMOTE** on training data only  

---

## Modeling & Evaluation
- Trained supervised classification models:
  - Logistic Regression  
  - Neural Network (TensorFlow / Keras)  
- Optimized decision thresholds for better recall–precision balance  
- Evaluated models using:
  - Accuracy  
  - Precision & Recall  
  - ROC–AUC  
  - Confusion Matrix  

---

## Key Insights
- Credit history is the strongest predictor of loan repayment  
- Income alone is not sufficient to assess credit risk  
- Class imbalance significantly affects baseline model performance  
- Threshold tuning improves default detection  

---

## Recommendation
Use the model as a **decision-support tool** rather than an automated approval system, combining predictions with human review for borderline cases.

---

## Data Preparation (ML-Ready)
- One-hot encoded categorical variables  
- Scaled numerical features  
- Applied SMOTE exclusively on training data to prevent data leakage  
- Split data into training, validation, and test sets  
- Final dataset prepared for future deployment and experimentation  

---

## Tools & Technologies
Python · pandas · numpy · matplotlib · seaborn · scikit-learn · TensorFlow · Keras

---

## Key Takeaway
Loan repayment behavior is driven primarily by **credit history and financial stability**, highlighting the importance of careful preprocessing, balanced datasets, and robust evaluation in credit risk modeling.

---

## About
**End-to-end machine learning project focused on credit risk analysis, classification modeling, and data-driven lending insights.**
