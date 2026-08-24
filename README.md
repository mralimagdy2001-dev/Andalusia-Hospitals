
📊 ## Andalusia Hospitals

## Healthcare Revenue & Operational Performance Analysis

📌 Project Overview
This project analyzes multi-facility medical billing and CRM data across hospital business units (AMH, ASH, HJH) in Egypt and the Kingdom of Saudi Arabia for Q1/Q2 2025. The purpose of this analysis is to evaluate operational throughput, compare baseline and historical targets against actual realized revenue, and uncover department-level performance drivers to optimize hospital financial health.

🎯 Business Problem
The organization faces target revenue shortfalls across multiple hospital units and medical departments, requiring clearer visibility into operational volume and payment performance.

## Key Business Questions

1) What is the overall performance? 
Actual revenue reached $552.38M out of a targeted $724.89M (76.2% target achievement).

2) Which products/customers/categories perform best? 
Inpatient ($150.91M actual) and Outpatient ($144.25M actual) lead revenue generation. Credit-based transactions account for 86.6% of overall revenue.

3) What are the main trends over time? 
Revenue peaked in April 2025 ($240.28M) before experiencing a sharp drop in May 2025 ($104.36M).

4) What factors are affecting business performance?
Lower volume realization in specialized critical care units (PICU, Open Heart, NICU) and target shortfalls in Credit collections directly impact total yield.

5) What actions can the business take based on the findings?
Reallocate capacity to high-margin departments (Inpatient, ICU), investigate May 2025 volume drop-offs, and improve credit contract optimization.

📂 Dataset
Source: Healthcare Billing, Marketing & Medical CRM Combined Dataset (Row Data.xlsx)

Time Period: March 2025 – May 2025

Main Tables / Columns:


🧹 Data Preparation
The dataset was prepared using:

Data cleaning: Imputed structural missing values across volume and average unit value (C/V) fields.

Handling missing values: Managed null values in non-volume departments (e.g., External Pharmacy Sales missing patient volume records).

Removing duplicates: Verified row uniqueness across country, unit, department, month, and payment type combinations.

Data type transformation: Standardized dates (Month converted to Date type) and numeric currency/volume formatting.

Creating calculated columns: Computed revenue variance (Actual Revenue - Target Revenue), achievement percentage, and price per unit metrics.

Creating relationships: Linked business units, geographical regions, and clinical departments to standardized dimension lookup tables.

Data modeling: Structured dynamic snowflake schema layout for efficient DAX performance.

🗂️ Data Model
1) Dim_BU
2) Department_Dim
3) Dim_Country
4) Payment_Dim
5) Billing Data
6) Marketing Data
7) Medical CRM Data

📊 Analysis & Dashboard
The project includes the following analysis areas:

## Overview

Total Actual Revenue: $552.38M

Total Target Revenue: $724.89M

Revenue Achievement: 76.2%

Historical Baseline Growth: +24.2% YoY ($552.38M vs. $444.61M Historical)

Department & Service Analysis

Top Performing: Inpatient ($150.91M), Outpatient ($144.25M), and ICU ($115.07M).

Underperforming: PICU (43.0% achievement), Open Heart (43.2% achievement), and NICU (50.0% achievement).

Payment & Unit Analysis

Credit Dominance: Credit transactions contributed $478.66M (86.6%) vs. Cash transactions at $73.72M (13.4%).

Facility Contribution: AMH facility generated $229.74M, ASH generated $186.00M, and HJH generated $136.63M.

Time & Growth Analysis

Peak Month: April 2025 delivered peak monthly actual revenue of $240.28M (97.4% target achievement).

Decline: May 2025 actual revenue dropped to $104.36M against a target of $238.27M (43.8% target achievement).

🔑 Key Insights
Insight 1 (Overall Target Gap): Across all business units, the organization realized an actual revenue target gap of $172.51M (-23.8% target deviation), despite achieving +24.2% growth over historical baseline figures.

Insight 2 (May 2025 Performance Drop): Actual revenue declined dramatically by 56.6% in May 2025 ($104.36M) compared to April 2025 ($240.28M), indicating a potential operational or recording gap in late Q2.

Insight 3 (Specialized ICU Shortfalls): Specialized intensive care services (PICU, NICU, Open Heart) missed revenue goals by over 50%, whereas standard Inpatient and Outpatient services maintained baseline operational volume.

💡 Business Recommendations
Focus on Specialized Bed Utilization: Investigate operational capacity bottlenecks, referral channels, and doctor availability in PICU, NICU, and Open Heart departments to improve unit conversion rate.

Audit Q2 Closing Data: Audit May 2025 billing cycle data to verify whether the revenue drop was driven by delayed credit approvals or unrecorded patient visits.

Optimize Credit Contract Yield: Given Credit accounts for 86.6% of overall revenue, renegotiate claim clearance terms and target thresholds with insurance providers.

🖼️ Dashboard Preview
Overview: Executive summary displaying KPI cards (Actual Revenue, Target Revenue, Achievement %), Country/BU revenue mapping, and monthly performance trend line.

Detailed Analysis: Department-level performance matrix, Payment Type breakdown, and Volume vs. Cost-per-Visit (C/V) scatter chart.

🛠️ Tools & Technologies
SQL: Data extraction and aggregation pipeline validation.

Power BI: Data visualization, interactive dashboarding, and report publication.

DAX: Calculated columns, time intelligence measures, and target achievement indicators.

Power Query: Data transformation, dynamic unpivoting, missing value management, and schema design.

Excel: Initial data exploration and file source format.




👤 Author
Ali Magdy

[GitHub](https://github.com/mralimagdy2001-dev) | [LinkedIn](https://www.linkedin.com/in/ali-magdy-mahmoud/)
