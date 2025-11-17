# Business Process Analysis for Customer Retention

### [Watch the Video Demo] | [View the Full PDF Case Study]

This is an end-to-end portfolio project analyzing customer churn for a telecom company. The goal was not just to build a report, but to build a complete system that analyzes *why* customers leave and *predicts* who will leave next, turning a reactive problem into a proactive business process.

---

## 🚀 The Business Problem
A telecom company was facing a high, undefined customer churn rate, leading to significant revenue loss. The business had customer data but no process to analyze it, creating a critical information gap:
* **No Root Cause:** They didn't know the primary drivers of churn (price, service, contract terms?).
* **No Clear Profile:** They couldn't identify *who* was leaving.
* **Reactive vs. Proactive:** All retention efforts were reactive, trying to win back customers *after* they had already left.

## 🎯 Project Objectives
1.  **Analyze** historical data to find the root cause of churn.
2.  **Monitor** current churn KPIs on a live Power BI dashboard.
3.  **Predict** which new customers are at high risk of churning in the future.

---

## 🛠️ Technologies Used
* **Database:** SQL Server
* **Data Transformation:** SQL, Power BI (Power Query)
* **Data Visualization:** Power BI
* **Predictive Modeling:** Python (Pandas, Scikit-learn, Random Forest)
* **IDE:** Jupyter Notebook

---

## 🔄 My End-to-End Process
[Raw Data (CSV)] ➔ [ETL in SQL Server] ➔ [Analysis in Power BI (Dashboard 1)] ➔ [Export Data] ➔ [Predictive Model in Python (Jupyter)] ➔ [Import Predictions] ➔ [Actionable Dashboard in Power BI (Dashboard 2)]

---

## 📊 Key Insights & Dashboards

### 1. Churn Analysis Dashboard
This dashboard serves as the main analysis tool for monitoring the health of the customer base.



* **Key Insight:** The "Month-to-Month" contract is the single biggest driver of churn. These customers have a **42.7% churn rate**, while "Two Year" contract customers only have a 2.8% rate.
* **Other Insights:**
    * Customers using "Fiber Optic" internet churn more (41.9%) than those on DSL (19.0%).
    * Customers who *don't* have "Online Security" or "Tech Support" are significantly more likely to leave.

### 2. Churn Prediction Dashboard
This dashboard is the final *solution*. It uses the Python model's predictions to show the *exact* list of new customers who are at high risk of churning, allowing the marketing team to target them with proactive retention offers (e.g., "Upgrade to a 1-Year contract for a 10% discount").


---

## 🤖 Predictive Model: Random Forest
A Random Forest Classifier was trained in Python to predict `Customer_Status` (Churned vs. Stayed).

* **Result:** The model achieved **84% accuracy** on the test set.
* **Top 5 Predictors (Feature Importance):**
    1.  `Contract` (Month-to-Month)
    2.  `Total Revenue`
    3.  `Total Charges` 
    4.  `Monthly_Charge`
    5.  `Total_Long_Distance_Charges` 

---

## 📂 Repository Structure
Customer-Retention-Analysis/
├── Data/
│   └── telecom_churn_data.csv
├── SQL_Scripts/
│   ├── 01_Create_Database.sql
│   └── 02_Clean_and_Transform.sql
├── Python_Model/
│   └── Churn_Prediction_Model.ipynb
├── Power_BI/
│   └── Customer Retention Dashboard.pbix
└── Business Process Analysis - Case Study.pdf

## Thank you so much for checking out my project. Hope you like it!
