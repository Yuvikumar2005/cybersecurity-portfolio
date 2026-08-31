# 🔎 Splunk Fraud Analysis Dashboard

## 📌 Overview

This project focuses on analyzing transaction data using Splunk Enterprise to identify fraudulent transaction patterns and present the findings through an interactive dashboard.

## 🎯 Objective

The main objective of this project was to ingest transaction data into Splunk, analyze fraudulent transactions using SPL queries, and create visualizations to identify patterns across different transaction attributes.

## 🛠️ Tools Used

- Splunk Enterprise
- SPL (Search Processing Language)
- CSV Dataset
- Splunk Dashboard

## 📊 Analysis Performed

The analysis focused on:

- Fraudulent transactions by category
- Fraudulent transactions by age group
- Fraudulent transactions by merchant
- Fraudulent transactions by gender
- Fraud trends across different transaction attributes

## 🔍 SPL Queries

### Fraud by Category

```spl
index=fraud_data fraud=1
| stats count by category
| sort - count

     Fraud by Gender
index=fraud_data fraud=1
| stats count by gender
| sort - count

      Fraud by Merchant 
index=fraud_data fraud=1
| stats count by merchant
| sort - count

      Fraud by Age
index=fraud_data fraud=1
| stats count by age
| sort - count
 ```
## 📈 Dashboard
The Splunk dashboard presents the analyzed fraud data using charts and tables to make important patterns easier to identify.

## 📄 Project Files
prepared_data(prepared_data).csv — Dataset used for analysis
Fraud Detection Dashboard.pdf — Exported Splunk dashboard
fraud_analysis_dashboard-pdf — Additional dashboard export

## 🧠 Skills Demonstrated
     Splunk Enterprise
     SPL query development
     Security data analysis
     Fraud pattern identification
     Data visualization
     Dashboard creation

## ⚠️ Disclaimer
This project was completed as a cybersecurity learning exercise using a training dataset. It is intended for educational and portfolio purposes only.
