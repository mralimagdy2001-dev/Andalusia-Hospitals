# Andalusia Hospitals

## 📊 Andalusia Hospitals - Directors High Level Dashboard
**Executive Healthcare & Digital Marketing Performance Dashboard**

---
## 📊 Dashboard Overview

---

## 📌 Project Overview
This project provides an integrated executive-level analysis of healthcare operations across multiple hospital business units (AMH, ASH, HJH) in Egypt and KSA. It consolidates clinical billing, digital marketing performance, and medical CRM pipelines to track revenue drivers, volume conversion rates, and department-level baseline growth.

---

## 🎯 Business Problem
The executive leadership needed visibility into why total revenue was missing targets and whether the deficit stemmed from clinical capacity, ineffective digital marketing funnels, or CRM conversion drops.

**Key Business Questions**
* **What is the overall performance?** Actual revenue reached $552M vs. $725M target (76% achievement, -23% Growth vs. Baseline).
* **How are Digital Marketing & CRM funnels performing?** Digital Marketing achieved only 48% of its revenue target ($73M / $151M), while Medical CRM achieved 73% ($75M / $102M).
* **Which departments face the biggest gaps?** Open Heart (43% Ach.), PICU (42% Ach.), and NICU (50% Ach.) showed severe target shortfalls.
* **What is driving the yield per procedure?** Despite lower volumes, Actual RPP / CPV outperformed targets ($13K in CRM vs $18K Target CPV scale, showing high unit value realization).
* **What actions should management take?** Re-align digital marketing spend towards high-yielding departments and resolve outpatient (OPD) volume conversion issues.

---

## 📂 Dataset
* **Source:** Integrated Hospital Enterprise Dataset (`Row Data.xlsx`)
* **Time Period:** March 2025 – May 2025
* **Main Tables / Columns:**
  * **Billing Data:** `Country Name`, `BU`, `Month`, `Unified Medical Department Name`, `Payment Type`, `Baseline/Actual/Target Revenue & Volume`
  * **Marketing Data:** `Digital Marketing Revenue`, `Volume`, `Target Revenue`, `Target Volume`, `CPV`
  * **Medical CRM Data:** `CRM Lead Revenue`, `Target CRM Revenue`, `Actual vs Target Volume`, `RPP`

---

## 🧹 Data Preparation
The dataset was prepared using:
* **Data cleaning:** Imputed null values across non-patient volume categories (e.g., External Pharmacy Sales).
* **Handling missing values:** Harmonized inconsistent department labels across CRM and Billing systems.
* **Removing duplicates:** Deduplicated cross-departmental patient logs.
* **Data type transformation:** Standardized dates and decimal currencies.
* **Creating calculated columns:** Calculated `Ach%` (Actual / Target), `G%` Growth vs. Baseline, and Revenue Variances.
* **Creating relationships:** Modeled star-schema connecting Billing, Marketing, and CRM to core Master Dimensions.
* **Data modeling:** Integrated multi-fact granularity handling.

---

## 🗂️ Data Model
* **Fact Billing Performance**
* **Fact Digital Marketing**
* **Fact Medical CRM**
* **Dim Date**
* **Dim Geography / Business Unit**
* **Dim Medical Department**

---

## 📊 Analysis & Dashboard
The project includes the following analysis areas:

1. **Executive Overview**
   * Total Revenue: **$552M Actual** | **$725M Target** (76% Ach., -23% G%)
   * OPD Volume: **172K Actual** | **244K Target** (71% Ach., -28% G%)
   * Total CPV: **4.1M Actual** | **4.5M Target** (90% Ach.)

2. **Digital Marketing Funnel**
   * Marketing Revenue: **$73M Actual** vs **$151M Target** (48% Ach.)
   * Marketing Volume: **54K Actual** vs **111K Target** (49% Ach.)
   * RPP Performance: **13K Actual** vs **13K Target** (98% Ach., +18% G%)

3. **Medical CRM Pipeline**
   * CRM Revenue: **$75M Actual** vs **$102M Target** (73% Ach.)
   * CRM Volume: **40K Actual** vs **58K Target** (69% Ach.)
   * CRM CPV Yield: **20K Actual** vs **18K Target** (113% Ach., +17% G%)

4. **Departmental Breakdown**
   * Top Contributors: Inpatient ($150.9M), Outpatient ($144.2M), ICU ($115.1M).
   * Lowest Target Achievement: Open Heart (43%), PICU (42%), NICU (50%).

---

## 🔑 Key Insights
* **Insight 1 (Digital Marketing Conversion Gap):** Digital Marketing missed its revenue goal significantly, achieving only $73M out of $151M (48% achievement), driven by a 51% shortfall in acquisition volume (54K vs 111K target).
* **Insight 2 (Strong Unit Realization - RPP/CPV):** While total volume failed to meet targets across all channels, average revenue per patient/procedure (RPP / CPV) was strong, exceeding targets in Medical CRM (113%) and reaching 98% in Digital Marketing.
* **Insight 3 (Critical Care Capacity Underutilization):** Highly specialized units (Open Heart at 43% achievement and PICU/NICU under 50%) are heavily dragging down total hospital performance.

---

## 💡 Business Recommendations
Based on the analysis:
* **Re-evaluate Digital Campaign Targeting:** Audit digital marketing acquisition channels to address the 51% lead/volume drop and reallocate ad budget toward high-converting clinical specialties.
* **Leverage High RPP/CPV Yield:** Since per-patient revenue yield is exceeding expectations (+17% to +18% growth), focus sales and CRM efforts on nurturing higher-intent patient leads.
* **Optimize Specialized Unit Referrals:** Investigate referral pathways for Open Heart, PICU, and NICU to raise throughput closer to baseline targets.

---

## 🖼️ Dashboard Preview
* **Overview:** High-level KPI cards for Total Revenue, OPD Volume, Marketing vs CRM Funnels, and Departmental drill-down matrix.
* **Detailed Analysis:** Deep-dive tabs for Payment Channel performance and monthly trends.

---

## 🛠️ Tools & Technologies
* **SQL** | **Power BI** | **DAX** | **Power Query** | **Excel** | **Python**

---

👤 Author
Ali Magdy

[GitHub](https://github.com/mralimagdy2001-dev/) | [LinkedIn](https://www.linkedin.com/in/ali-magdy-mahmoud/)
