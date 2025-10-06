# Telco Customer Churn Analysis & Prevention Dashboard

This repository contains the Power BI project file and documentation for a churn analysis dashboard designed to help a telecommunications company understand and reduce customer attrition.

![Dashboard GIF Preview](Dashboard_Preview_v2.gif)

---

## 🎯 The Business Problem

**Connectra Telecom**, a fictional telecommunications provider, has been facing a significant challenge with customer churn. A high rate of customer attrition was impacting revenue, increasing acquisition costs, and hindering long-term growth.

The leadership team lacked clear, data-driven insights into **why** customers were leaving and **who** was most at risk. Decisions regarding retention campaigns were being made based on intuition rather than evidence.

This project aims to solve this problem by providing a business intelligence solution that:
1.  **Diagnoses** the primary drivers of customer churn.
2.  **Identifies** the key profiles and segments of customers who are most likely to leave.
3.  **Provides** actionable recommendations for the marketing and customer success teams to improve retention.

## 📊 Data Source

The dataset used for this analysis is the **"Telco Customer Churn"** dataset, publicly available on Kaggle. It contains customer account information, demographic data, and services subscribed to.

- **Source:** [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## 📈 Key Insights

The analysis revealed several critical factors that strongly correlate with customer churn:

1.  **Contract Type is the #1 Churn Predictor:** Customers on **Month-to-Month contracts have a churn rate of 42.7%**, which is dramatically higher than those on One-Year (11.3%) or Two-Year (2.8%) contracts. This flexibility comes at the cost of loyalty.

2.  **New Customers are Highly Vulnerable:** The churn rate is highest among customers with a tenure of less than 12 months, suggesting potential issues in the initial **onboarding process** and the customer's ability to realize the service's full value early on.

3.  **Internet Service Matters:** Customers with **Fiber Optic internet service exhibit a significantly higher churn rate (41.9%)** compared to those with DSL (19%). This may indicate service stability issues, pricing dissatisfaction, or stronger competition in areas with fiber coverage.

4.  **Billing Methods Signal Risk:** Customers using **Paperless Billing** and paying via **Electronic Check** are more likely to churn. This could signal friction in the payment process or a less "sticky," more transactional customer relationship.
