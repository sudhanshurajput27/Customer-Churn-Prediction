# Customer Churn Prediction

## Overview
This project builds a machine learning pipeline to predict which customers 
are likely to cancel their subscription (churn) in the near future. 
We used various models like Logistic regression, Random Forest and XGBoost
and then delected the best one after which we created a explainabiltiy to explain how each data 
work to people from a business perspective

---

---

## Dataset
- **Source:** [IBM Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Size:** 7,043 customers, 21 features
- **Target:** `Churn` — whether the customer left in the last month (Yes/No)
- **Features include:** customer demographics, services subscribed, 
contract type, payment method, monthly and total charges

### Top Churn Drivers (SHAP Analysis)
1. **Tenure** — shortest tenure customers are at highest churn risk
2. **Contract Type** — month-to-month customers churn significantly more 
than one or two year contract customers
3. **Internet Service** — fiber optic customers churn at higher rates 
despite having a premium service, likely due to higher costs
4. **Payment Method** — electronic check users show higher churn tendency
5. **Monthly Charges** — higher charges correlate with increased churn risk

---

## Key Findings
- New customers (low tenure) are the highest churn risk group
- Month-to-month contracts are the strongest retention lever — 
moving customers to annual contracts significantly reduces churn
- Fiber optic customers need targeted retention despite being 
premium subscribers
- Customers without add-on services (Online Security, Tech Support) 
churn more — bundling may improve retention

