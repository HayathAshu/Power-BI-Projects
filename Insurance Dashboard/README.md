# 📊 Insurance Claims Analysis Dashboard (Power BI)

## 📌 Project Overview
This project focuses on analyzing and visualizing insurance claims data using **Microsoft Power BI**.  
The dashboard provides a comprehensive view of claim trends, financial performance, and risk factors to help insurance leadership make data-driven decisions.

The analysis is based on insurance claims processed during **January and February**, covering customer, policy, vehicle, and incident details.

---

## 🧠 Problem Statement
An insurance company wants to **visualize the financial performance of claims made against its policies** and gain insights into:

- Total claims and approved claim amounts  
- Claim distribution across states  
- Impact of vehicle age, gender, and time of day on claims  
- Identification of high-risk segments that lead to higher claim frequency and payouts  

The goal is to create an **interactive dashboard** that gives leadership a **quick, clear, and actionable overview** of insurance claims data.

---

## 📂 Dataset Information
- **Total Records:** 1,000 insurance claims  
- **Time Period:** January & February  
- **File Name:** `insurance.csv`

### Key Dataset Characteristics:
- Each claim contains **~40 attributes**
- Attributes fall into four major categories:
  - **Insured Person Details**
  - **Policy Information**
  - **Incident Description**
  - **Vehicle Characteristics**
- Key variable of interest:
  - `fraud_reported`  
    - `1` → Fraudulent claim  
    - `0` → Non-fraudulent claim  

---

## 🛠 Tools & Technologies Used
- **Microsoft Power BI**
- **DAX (Data Analysis Expressions)**
- **Data Cleaning & Transformation**
- **Data Visualization**

---

## 📊 Dashboard Features
The Power BI dashboard includes the following key metrics and visualizations:

### 🔢 KPI Cards
- Average Vehicle Age  
- Total Number of Claims  
- Total Approved Claim Amount  
- Total Injury Claim Amount  
- Total Number of Vehicles Involved  

### 🌍 Geographical Analysis
- Claims distribution by **Policy State** (Map Visualization)

### 📈 Analytical Visuals
- **Claims by Gender** (Donut Chart)
- **Total Claims by Vehicle Age** (Bar Chart)
- **Claims by Hour of the Day** (Line Chart)
- **Number of Claims by State** (Bar Chart)

### 🎛 Interactive Filters
- Policy State  
- Incident Type  
- Insured Gender  

These slicers allow dynamic analysis and deeper insights.

---

## 🧮 Key DAX Measure Used
```DAX
Profit = 
SUM(insurance[policy_annual_premium]) 
- SUM(insurance[total_claim_amount])
```
---

## 🔍 Key Insights
1️⃣ Claims by State

- States such as California, Oregon, and Nevada show:

- Highest number of claims

- Highest total approved claim amounts

- Likely reasons:

- Higher population density

- Increased traffic and accident rates

2️⃣ Time, Gender & Vehicle Age Impact

- Claims peak during late evening hours (5 PM – 9 PM)

- Male policyholders report slightly more claims than females

- Older vehicles (pre-2010) are associated with:

- Higher claim frequency

- More severe accidents

---

## 🔮 Future Scope

- Fraud detection modeling using fraud_reported

- Predictive analytics for claim forecasting

- Risk scoring for customers and vehicles

- Integration with machine learning models

---

## 📁 Repository Structure
```
├── Insurance Proposal.pdf
├── insurance.csv
├── Insurance_Dashboard.pbix
├── Insrance_Dashboard_ScreenShot.png
└── README.md
```
---

## ✅ Conclusion

This project demonstrates how Power BI dashboards can transform raw insurance data into meaningful insights, enabling better decision-making, improved risk management, and enhanced financial performance tracking.

---

## 👤 Author
**Name:** Mohammed Hayath R K  
**Role:** Data Analyst
**Tools:** Power BI, DAX, SQL, Data Visualization  
