# Home_Loan_Project_Joana_Coyle
# Sales Performance Analysis — Joana Coyle

## Overview
Sales performance analysis using **exploratory data analysis (EDA) and data visualization** to identify regional trends, uncover low-performing states, and support data-driven sales and marketing strategies.

---

## Dataset
- **7,560 records** of Australian apparel sales  
- **Time period:** Q4 2020 (October–December)  
- **Key features:**  
  - Date  
  - Time of Day  
  - State  
  - Customer Group  
  - Units Sold  
  - Sales  

> Note: All data falls within a single quarter, so quarterly comparisons are not meaningful.

---

## Workflow

### Data Wrangling & Validation
- Verified absence of missing values and duplicates  
- Preserved an untouched copy of the original dataset  
- Converted date fields to datetime format  
- Engineered time-based features:
  - Week  
  - Month  
  - Month Name  

### Exploratory Data Analysis (EDA)
- Identified a right-skewed sales distribution with high-value outliers  
- Confirmed a strong positive relationship between **Units Sold** and **Sales**  
- Analyzed sales performance by:
  - State  
  - Customer Group  
  - Time of Day  
  - Week and Month  

### Regional Analysis
- **Top-performing states:** VIC, NSW, SA  
- **Lowest-performing states:** WA, NT, TAS, QLD  
- Time of day and customer group showed **minimal influence** on low performance  
- **November** identified as the weakest sales month across all states  

---

## Key Insights
- Higher unit sales consistently result in higher revenue  
- Sales patterns remain stable across time of day and customer groups  
- Seasonality is the primary driver of sales variation  
- November underperforms despite marking the beginning of the holiday season  

---

## Recommendation
Implement a **targeted November marketing campaign** to encourage earlier holiday shopping and improve revenue during a consistently weak sales period.

---

## Data Preparation (ML-Ready)
- Converted dates to numeric timestamps  
- Applied one-hot encoding to categorical variables  
- Normalized numerical features using **MinMaxScaler**  
- Final dataset prepared for downstream machine learning applications  

---

## Tools & Technologies
- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

---

## Key Takeaway
Sales performance differences are driven more by **seasonality and sales volume** than by customer segment or time of day, highlighting November as a critical opportunity for revenue growth.

---

## About
**Exploratory data analysis and visualization project focused on sales performance, regional trends, and data-driven marketing insights.**
