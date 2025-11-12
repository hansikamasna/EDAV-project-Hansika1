# 📊 Telecom Customer Churn Prediction

**Using Machine Learning to Reduce Customer Attrition**

A data-driven project aimed at predicting customer churn in the telecom industry using advanced machine learning techniques.  
Developed by **Masna Hansika**  
📅 *Date: 10 Nov 2025*

---

## 🧩 Project Overview

Customer churn — when customers stop using a company’s services — is a critical problem in the telecom industry.  
Acquiring new customers is **5–25x more expensive** than retaining existing ones.  

This project builds an **end-to-end ML pipeline** to:
- Identify **at-risk customers** before they leave.  
- Enable **data-driven retention strategies**.  
- Provide **real-time churn predictions**.

---

## 🧠 Key Highlights

| Metric | Value |
|---------|--------|
| Model Accuracy | **88%** |
| Dataset Size | **1000+ Customers** |
| Churn Rate | **~27%** |
| Features Used | **21 Features → 45+ after encoding** |
| Algorithms Compared | 6 Models |
| Best Model | **Random Forest (ROC-AUC = 0.88)** |

---

## 📁 Dataset Information

**Source:** [Telco Customer Churn Dataset (Kaggle)](https://www.kaggle.com/blastchar/telco-customer-churn)

### Feature Categories:
1. **Account Info (6):** Tenure, Contract, Billing, Payment, Monthly & Total Charges  
2. **Demographics (5):** Gender, Senior Citizen, Partner, Dependents, Customer ID  
3. **Services (9):** Phone, Internet, Security, Backup, Protection, Tech Support, Streaming  
4. **Target Variable (1):** `Churn` (Yes/No)

---

## 🔄 Project Pipeline

1. **Data Collection** – Import dataset from Kaggle or local source  
2. **Data Preprocessing** – Handle missing values, encode categories, and scale features  
3. **Exploratory Data Analysis (EDA)** – Visualize distributions, correlations, and patterns  
4. **Feature Engineering** – Create new metrics like `ChargePerTenure` and `TenureGroup`  
5. **Model Training & Comparison** – Evaluate six algorithms  
6. **Model Evaluation & Insights** – Select best model and interpret key results

---

## ⚙️ Preprocessing Details

- **Missing Value Handling:**  
  - *Numerical:* Median imputation  
  - *Categorical:* Mode imputation  
  - `TotalCharges` converted to numeric  

- **Encoding:**  
  - Binary Encoding: Yes/No → 1/0 (15 features)  
  - One-Hot Encoding for multi-category columns  

- **Scaling:**  
  - Used `StandardScaler` (mean = 0, std = 1)

- **Feature Engineering:**  
  - `ChargePerTenure = MonthlyCharges / Tenure`  
  - `TenureGroup` created (e.g., Short-Term, Mid-Term, Long-Term)

---

## 📊 Exploratory Data Analysis (EDA)

### Key Findings:
- **Churn Distribution:** 27% customers churned  
- **Correlations with Churn:**
  - 📉 Low tenure → -0.35 correlation  
  - 🌐 Fiber optic internet → +0.31 correlation  
  - 💳 Electronic check payment → +0.28 correlation  
  - 📅 Month-to-month contract → +0.45 correlation  

*(Include screenshots of EDA visualizations if available)*

---

## 🤖 Model Training & Evaluation

### Models Compared:
| Algorithm | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|------------|-----------|------------|---------|-----------|----------|
| Random Forest | **0.82** | **0.71** | 0.58 | 0.64 | **0.88** |
| XGBoost | 0.81 | 0.70 | 0.58 | 0.64 | 0.87 |
| Gradient Boosting | 0.80 | 0.69 | 0.56 | 0.62 | 0.86 |
| LightGBM | 0.80 | 0.68 | 0.55 | 0.61 | 0.84 |
| Logistic Regression | 0.79 | 0.67 | 0.54 | 0.60 | 0.84 |
| Decision Tree | 0.75 | 0.60 | 0.54 | 0.59 | 0.78 |

### 🏆 Best Model: Random Forest Classifier
- **Accuracy:** 82%  
- **Precision:** 71%  
- **Recall:** 58%  
- **ROC-AUC:** 0.88  

---

## 🎯 Business Insights

- Customers with **month-to-month contracts** or **electronic check payments** are more likely to churn.  
- **Longer tenure** customers show strong loyalty.  
- Promoting **annual contracts** and **automatic payments** can reduce churn significantly.

---

## 🧰 Tech Stack

- **Programming Language:** Python  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, lightgbm  
- **Tools:** Jupyter Notebook / Google Colab  
- **Dataset:** Kaggle (Telco Customer Churn)

---

## 🚀 Future Scope

- Integrate with **real-time dashboards** (using Streamlit or Power BI).  
- Deploy model with **Flask API** for live predictions.  
- Add **deep learning models** for improved recall.  
- Perform **SHAP-based model explainability** for interpretability.

---

## 📬 Contact

**Author:** Masna Hansika  
📧 Email: *(add your email if you want)*  
📆 Date: 10 Nov 2025  

---
