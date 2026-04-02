# 🏗️ DPWH Infrastructure Performance Analysis
**An End-to-End Data Engineering & Visualization Project**

## 📌 Executive Summary
This project analyzes **206,003** infrastructure projects from the Department of Public Works and Highways (DPWH). I transformed raw, high-volume government data into a structured format to track ₱4.58 Trillion in budget allocation and contractor performance.

### 📊 Dashboard Preview
![DPWH Dashboard](DPWH_Dashboard_Final.png)

## 🛠️ Technical Stack
* **Data Engineering:** Python (Pandas) for ETL, missing value imputation, and data validation.
* **Database Logic:** Feature engineering for project duration and status normalization.
* **BI & UI/UX:** Tableau Desktop and Canva for executive-level storytelling.

## 🧹 Data Pipeline & Integrity (The "DBA" Approach)
As a future Database Administrator, I prioritized data quality over simple visualization. My Python pipeline handled:
* **Constraint Validation:** Identified and removed "time-travel" records where completion dates preceded start dates (negative durations).
* **Null Management:** Imputed 6,500+ missing categorical values to prevent "orphaned" records in the final reporting.
* **Efficiency Metrics:** Engineered the `projectDuration_days` column to provide a quantifiable KPI for project bottlenecks.

## 💡 Key Business Insights
* **Budget Concentration:** Road infrastructure dominates national spending at **₱2.08 Trillion**.
* **Project Velocity:** Foreign-Assisted Projects (FAPs) average **1,200+ days** for completion, highlighting significant logistical or bureaucratic overhead compared to local funding.
* **Contractor Load:** The Top 15 contractors manage a disproportionate volume of the total workload, indicating a centralized market.

---
*Data Source: Open Portal by BetterGov.ph*
