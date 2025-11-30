# 🔍 Proactive Employee Attrition Prediction System

A Machine Learning–powered HR analytics solution designed to **predict employee turnover** and help organizations proactively retain top talent.

---

## 📌 Overview

Employee attrition increases hiring costs, disrupts business continuity, and lowers company morale.  
Our system uses **data-driven insights** to:

✔ Predict whether an employee is at risk of leaving  
✔ Identify key drivers behind attrition  
✔ Enable proactive HR retention strategies  

---

## ✨ Key Features

- Employee attrition prediction using **XGBoost**
- Employee segmentation using **K-Means Clustering**
- Comprehensive HR analytics dashboard *(planned deployment UI)*
- ML model lifecycle management using **MLflow**
- FastAPI backend for prediction serving

🖼️ *Placeholder for Dashboard Screenshot*  
> A UI dashboard showing employee input form and predicted attrition risk.

---

## 🧰 Tools & Technologies

| Category | Tools |
|---------|------|
| ML | XGBoost, Scikit-learn, K-Means |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Backend | FastAPI |
| MLOps | MLflow |
| IDEs | Google Colab, Jupyter Notebook |

---

## 📊 Dataset Summary

We used a **large HR dataset** with ~**250K** employee records and **17 features**, including:

- Demographics (Age, Marital Status)
- Work environment metrics (Distance From Home, Job Level)
- Satisfaction ratings
- Compensation and promotion history

🖼️ *Placeholder for Dataset Head Preview*  
> First 5 rows table showing dataset structure.

---

## 🔎 Exploratory Data Analysis (EDA)

EDA helped reveal patterns influencing attrition such as low pay, overtime, satisfaction levels, and career stagnation.

### 🔹 Attrition Distribution
<img width="402" height="409" alt="image" src="https://github.com/user-attachments/assets/4279a36d-d2c8-43c4-8429-34ae49d6668b" />

> Shows that the percentage of employees who left is significantly lower than those who stayed, indicating a class imbalance.

---

### 🔹 Attrition vs Numerical Features
<img width="589" height="453" alt="image" src="https://github.com/user-attachments/assets/a0a38a9f-9f52-4bbf-8168-f81499e22d3f" />
<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/d4e7b599-fe89-4611-88a1-5adc0b4c6074" />

> Boxplots reveal employees who leave often have **lower satisfaction and income**.

---

### 🔹 Correlation Heatmap
<img width="2737" height="2490" alt="image" src="https://github.com/user-attachments/assets/02320caf-b5fe-49dd-ad0e-0fae18469c22" />

> Helps identify important predictive relationships such as:
- High correlation between **overall happiness** & retention
- Work-life balance & overtime influence attrition

---

## 🔧 Data Preprocessing & Feature Engineering

✔ Missing value imputation  
✔ Removal of duplicate records  
✔ Binary Encoding (Attrition, OverTime)  
✔ Ordinal Encoding (BusinessTravel)  
✔ One-hot encoding of Department & Marital Status  

### ✨ Engineered Features
| Feature | Meaning |
|--------|---------|
| PromotionLethargy | Slow promotions lead to dissatisfaction |
| HighDistanceLowPay | Low salary + long commute increases leave risk |
| WorkLifeCommuteStrain | Work-life balance vs travel burden |
| OverallHappinessScore | Combined satisfaction score |


---

## 🤖 Machine Learning

Multiple models evaluated:

| Model | Status |
|------|-------|
| Logistic Regression | Tested |
| KNN | Tested |
| Random Forest | Tested |
| **XGBoost** | ✔ Best model — selected for deployment 🎯 |

### Final Architecture
🖼️ *Architecture Diagram Placeholder*  
> Flow: Data ➜ Preprocessing ➜ MLflow Tracking ➜ XGBoost Model ➜ FastAPI Service ➜ Frontend UI (planned)

---

## 🧩 Employee Segmentation

We applied **K-Means clustering** to group employees into risk profiles.  
Useful for HR action targeting:  
✔ High-risk low-satisfaction group  
✔ Hard-working but underpaid group  
✔ Stable & satisfied employees  

<img width="1175" height="1195" alt="image" src="https://github.com/user-attachments/assets/aa764227-c1a2-4651-b8f1-1bf17b07163b" />

---

## 🚀 Deployment

The trained model is tracked via **MLflow** and served using **FastAPI** as a prediction API.

🖼️ *FastAPI Endpoint Screenshot Placeholder*  
> Example JSON response for prediction request.

---

## 🧪 Statistical Significance Testing

| Test | Result | Meaning |
|------|--------|---------|
| T-test (JobSatisfaction vs Attrition) | ❗ Significant | Job satisfaction strongly affects turnover |
| Chi-Square (Overtime vs Attrition) | ❗ Significant | Overtime workers leave more |

---

## 🧱 Repository Structure
```
📂 Employee-Attrition-Prediction-and-Analysis
├── 📁 EDA & Encoder Notebooks
├── 📁 Clustering Notebook
├── 📁 Model + MLflow Artifacts
├── 📁 FastAPI Deployment Files
├── 📄 README.md (this file)
└── 📄 Dataset CSVs
```

---

## 👥 Team Members

- Ahmed Fekry Mohamed  
- Yousif Moaz Elbadry  
- Mazen Kamal Morsy  
- Shaimaa Ahmed Fouad  
- Youssef Ahmed Fouad  

---

## 🚀 Future Enhancements

- Fully hosted frontend dashboard
- SHAP explainability for HR interpretation
- Live employee data streaming + auto retraining
- Role-based access for HR management

---

## ⭐ Support

If you found this project insightful —  
please **Star ⭐ this repository** and follow for more!

---
