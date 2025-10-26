# Telco Customer Churn Analysis & Prevention Dashboard

This repository contains the Power BI project file and documentation for a churn analysis dashboard designed to help a telecommunications company understand and reduce customer attrition.

![Dashboard GIF Preview](Dashboard_Preview_v2.gif)


## 🎯 The Business Problem

**Connectra Telecom**, a fictional telecommunications provider, has been facing a significant challenge with customer churn. A high rate of customer attrition was impacting revenue, increasing acquisition costs, and hindering long-term growth.

The leadership team lacked clear, data-driven insights into **why** customers were leaving and **who** was most at risk. Decisions regarding retention campaigns were being made based on intuition rather than evidence.

This project aims to solve this problem by providing a business intelligence solution that:
1.  **Diagnoses** the primary drivers of customer churn.
2.  **Identifies** the key profiles and segments of customers who are most likely to leave.
3.  **Provides** actionable recommendations for the marketing and customer success teams to improve retention.

## 📊 Data Source

The dataset used for this analysis is the **"Telco Customer Churn"** dataset, publicly available on Kaggle. It contains customer account information, demographic data, and services subscribed to.

**Source:** [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)


## 📈 Key Insights

The analysis revealed several critical factors that strongly correlate with customer churn:

1.  **Contract Type is the #1 Churn Predictor:** Customers on **Month-to-Month contracts have a churn rate of 42.7%**, which is dramatically higher than those on One-Year (11.3%) or Two-Year (2.8%) contracts. This flexibility comes at the cost of loyalty.

2.  **New Customers are Highly Vulnerable:** The churn rate is highest among customers with a tenure of less than 12 months, suggesting potential issues in the initial **onboarding process** and the customer's ability to realize the service's full value early on.

3.  **Internet Service Matters:** Customers with **Fiber Optic internet service exhibit a significantly higher churn rate (41.9%)** compared to those with DSL (19%). This may indicate service stability issues, pricing dissatisfaction, or stronger competition in areas with fiber coverage.

4.  **Billing Methods Signal Risk:** Customers using **Paperless Billing** and paying via **Electronic Check** are more likely to churn. This could signal friction in the payment process or a less "sticky," more transactional customer relationship.

## 🔧 Project Versioning with .pbip

This project is saved using the **Power BI Project (`.pbip`)** format rather than the standard `.pbix` file. This approach is essential for effective version control with Git and GitHub.

The `.pbip` format stores the project as a folder containing human-readable, text-based files, most importantly:

* **`Report.json`**: Defines all report pages, visuals, and layouts.
* **`Model.bim`**: A JSON-based file (Tabular Model Scripting Language) that defines the data model, tables, relationships, and all DAX measures.

**Key Advantages of this format:**
* **Granular Change Tracking:** Git can track the exact changes made to the data model (like a modified DAX measure in `Model.bim`) or the report (like a moved visual in `Report.json`).
* **Meaningful Diffs:** We can see clear "diffs" between commits, making it possible to review changes and understand the project's history.
* **Collaboration:** This text-based structure is "Git-friendly" and significantly reduces issues with merge conflicts, allowing for better team collaboration.
* **Clean Repository:** A `.gitignore` file is used to exclude user-specific local settings (like `.pbi/localSettings.json`), keeping the repository focused only on the core project files.