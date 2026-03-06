# Customer-Churn-Prediction-Model-CLV-Based-Retention-Strategy

## 📌 Project Overview

Customer churn is a major challenge for subscription-based businesses. Retaining existing customers is often significantly cheaper than acquiring new ones, making churn prediction a critical analytics problem.

This project builds an **end-to-end churn prediction and customer lifetime value (CLV) analysis system** using machine learning. The goal is to identify high-risk customers and estimate the financial impact of targeted retention strategies.

The solution combines **predictive modeling, customer segmentation, and ROI simulation** to help businesses make data-driven retention decisions.

---

## 🎯 Business Objectives

The project addresses three key business questions:

1. **Which customers are likely to churn?**
2. **Which customers are the most valuable to the business?**
3. **Which customers should be prioritized for retention campaigns to maximize ROI?**

By answering these questions, companies can **target retention efforts more effectively and reduce revenue loss from churn.**

---

## 📊 Dataset

The project uses the **Telco Customer Churn dataset**, which contains customer information such as:

* Demographics
* Contract details
* Internet services
* Billing information
* Customer tenure
* Payment methods

Dataset size:

* **7043 customers**
* **30+ features**

Target variable:

* **Churn (Yes / No)**

---

## 🛠 Tech Stack

**Tech Used:**
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Power BI, Machine Learning, Predictive Analytics

---

## ⚙️ Project Workflow

### 1. Data Cleaning & Preparation

* Handled missing values in `TotalCharges`
* Encoded categorical features
* Removed non-informative identifiers
* Prepared dataset for modeling

### 2. Exploratory Data Analysis (EDA)

Key insights discovered:

* **Month-to-month contracts show significantly higher churn**
* **Electronic check users have the highest churn rate**
* **Customers with shorter tenure are more likely to churn**
* **Higher monthly charges correlate with increased churn risk**

These insights helped guide feature selection and modeling.

---

### 3. Churn Prediction Model

Two machine learning models were trained and compared:

**Logistic Regression**

* ROC-AUC: **0.84**
* Churn Recall: **56%**

**Random Forest (Final Model)**

* ROC-AUC: **0.84**
* Churn Recall: **74%**

Random Forest was selected as the final model because it **identifies significantly more churn-risk customers**, which is crucial for retention strategies.

---

### 4. Key Churn Drivers

Feature importance analysis revealed the most influential churn factors:

* Customer tenure
* Total charges
* Monthly charges
* Contract type
* Fiber optic internet service
* Payment method

These variables provide actionable insights into customer behavior and retention risk.

---

### 5. Customer Lifetime Value (CLV) Analysis

Customer Lifetime Value was estimated using:

CLV = Monthly Charges × Expected Remaining Lifetime

Customers were segmented into:

* Low Value
* Medium Value
* High Value
* Very High Value

This segmentation enables businesses to focus on **retaining the most valuable customers first.**

---

### 6. Risk-Based Customer Segmentation

Customers were categorized based on:

* **Churn Probability**
* **Customer Lifetime Value**

This allowed identification of the **most critical group**:

**High CLV + High Churn Risk**

Result:

* **187 high-value customers identified as at risk**

---

### 7. Retention Campaign ROI Simulation

To evaluate business impact, a retention campaign was simulated.

Assumptions:

* Retention campaign cost: **₹500 per customer**
* Expected churn reduction: **25%**

Results:

| Metric                 | Value    |
| ---------------------- | -------- |
| Priority Customers     | 187      |
| Revenue at Risk        | ₹418,107 |
| Campaign Cost          | ₹93,500  |
| Expected Revenue Saved | ₹104,526 |
| Net ROI                | ₹11,026  |

This demonstrates that **targeted retention campaigns can generate positive financial returns.**

---

## 📈 Dashboard (yet to come)

A Power BI dashboard was created to visualize:

* Customer churn overview
* Churn drivers
* CLV distribution
* High-risk customer segments
* Revenue impact and ROI simulation

The dashboard enables stakeholders to **interactively explore churn risks and prioritize retention strategies.**

---

## 📁 Project Structure

```
customer-churn-clv-prediction
│
├── data
│
├── notebooks
│   ├── data_cleaning.ipynb
│   ├── exploratory_analysis.ipynb
│   ├── churn_modeling.ipynb
│   └── clv_roi_analysis.ipynb
│
├── dashboard
│   └── powerbi_dashboard.pbix
│
└── README.md
```

---

## 🚀 Key Outcomes

* Built an end-to-end churn prediction system with **ROC-AUC 0.84**
* Identified **13% of customers as high-value churn risks**
* Estimated **₹418K revenue exposure**
* Demonstrated **positive ROI from targeted retention strategies**

---

## 💡 Future Improvements

Potential enhancements include:

* Implementing advanced models (XGBoost, LightGBM)
* Deploying the model using an API or web app
* Automating real-time churn monitoring
* Integrating customer support and usage data

---

## 👤 Author

Nikita Chaudhary
Data Science & Machine Learning Enthusiast
