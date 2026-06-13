# IBM HR Attrition Analysis

![SQL](https://img.shields.io/badge/SQL-MySQL-blue)
![Python](https://img.shields.io/badge/Python-Pandas%20%7C%20Seaborn-yellow)
![PowerBI](https://img.shields.io/badge/PowerBI-Dashboard-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Overview
End-to-end HR analytics project analysing IBM's HR Attrition dataset 
(1,470 employees, 35 columns) to uncover key attrition drivers and 
workforce patterns. Built across three layers — SQL for structured 
querying, Python/Jupyter for EDA and visualization, and Power BI 
for interactive dashboard reporting.

---

## Project Workflow
Raw Data → SQL Analysis → Python EDA (Jupyter) → Power BI Dashboard

---

## Key Business Insights

1. **Overtime Strongly Impacts Attrition** — Employees working overtime
   showed significantly higher attrition, indicating burnout as a major driver
2. **Sales Department Has Highest Attrition** — Highest turnover among
   all departments, likely driven by targets and high-pressure environment
3. **Lower Salary = Higher Attrition** — Compensation satisfaction plays
   a key role in employee retention
4. **Younger Employees (25–35) Leave More** — Likely seeking faster
   career growth and better opportunities
5. **Poor Work-Life Balance Affects Retention** — Lower work-life balance
   ratings correlated with higher attrition
6. **Single Employees Show Higher Attrition** — Compared to married
   and divorced employees
7. **Short Tenure Employees Leave More Frequently** — Possible gaps
   in onboarding and early engagement
8. **Sales Executives and Lab Technicians** have highest attrition
   by job role

---

## Dashboard Preview
![Dashboard](dashboard/dashboard_screenshot.png)

---

## Tools & Techniques

| Layer | Tool | What Was Done |
|---|---|---|
| Data Querying | MySQL | CASE bucketing, conditional aggregation, department distribution |
| Exploratory Analysis | Python / Jupyter | Pandas, Seaborn, Matplotlib — EDA and 8+ visualizations |
| Visualization | Power BI | Interactive dashboard, KPI cards, attrition breakdowns |

---

## SQL Queries Included

| Query | Technique Used |
|---|---|
| Categorize employees into salary bands | CASE WHEN bucketing |
| Attrition count by marital status | Conditional aggregation (single row) |
| Male vs Female avg salary by department | CASE inside AVG(), GROUP BY |
| Department-wise employee distribution % | Subquery, ROUND(), percentage calc |

---

## Python / Jupyter Notebook Covers

- Dataset loading and inspection (shape, dtypes, describe)
- Null value and duplicate check — dataset confirmed clean
- Overall attrition rate calculation
- Average monthly income and average age
- Visualizations:
  - Attrition count
  - Department-wise attrition
  - Overtime vs attrition
  - Salary distribution (histogram + KDE)
  - Age distribution
  - Correlation heatmap
  - Attrition by job role
  - Work-life balance vs attrition
- Attrition percentage by department (crosstab)
- Average income by job role
- Overtime attrition rate

---

## Dataset
- **Source:** IBM HR Analytics Employee Attrition & Performance
  ([Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset))
- **Records:** 1,470 employees | 35 columns

---

## How to Run

**SQL:**
1. Import CSV into MySQL Workbench
2. Run `sql/ibm_sql_hr.sql` query by query

**Jupyter Notebook:**
1. Open `notebooks/IBM_HR.ipynb`
2. Place the CSV in the same folder
3. Run all cells (requires pandas, numpy, seaborn, matplotlib)

**Power BI:**
1. Open `dashboard/IBM_HR.pbix` in Power BI Desktop
2. Refresh data source if prompted
3. See `dashboard/dashboard_screenshot.png` for preview

---

## Project Structure
