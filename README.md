<div align="center">

#  Payroll Analytics Dashboard

### End-to-End Power BI Dashboard for Multi-Year Employee Payroll Analysis

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-217346?style=flat-square&logo=microsoft&logoColor=white)
![SQL](https://img.shields.io/badge/Oracle%20SQL-F80000?style=flat-square&logo=oracle&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)

</div>


##  Table of Contents

- [Project Overview](#-project-overview)
- [Sample Dataset](#-sample-dataset)
- [Tools & Technologies](#-tools--technologies)
- [Dashboard Pages](#-dashboard-pages)
- [Analytical Approach](#-analytical-approach)
- [Data Cleaning Steps](#-data-cleaning-steps)
- [Data Model](#-data-model)
- [DAX Measures](#-dax-measures)
- [Sample Insights](#-sample-insights-illustrative)
- [Data Quality](#-data-quality)
- [Key Skills Demonstrated](#-key-skills-demonstrated)
- [Author](#-author)

---

##  Project Overview

This project transforms a large, multi-year raw payroll dataset into an interactive, multi-level **Power BI** dashboard — from company-wide trends down to individual employee-level analysis. Built end-to-end: data cleaning in Power Query, relational data modelling, DAX measure design, and a 10-page interactive report with drill-through navigation.

| Metric (illustrative) | Value |
|---|---|
| Time Period Covered | 5 years |
| Zones Analyzed | 10 |
| Departments Analyzed | 250+ |
| Salary Categories | 7 |
| Dashboard Pages | 10 |

---

##  Sample Dataset

| Column | Type | Description |
|--------|------|--------------|
| `SALARY_DATE` | Date | Monthly payroll date |
| `ZONE` | Text | Factory/site zone code |
| `SALARY_GROUP` | Text | Employee category (worker, staff, executive, etc.) |
| `DEPARTMENT` | Text | Department name |
| `EMPLOYEE_CODE` | Text | Unique employee identifier |
| `EMPLOYEE_NAME` | Text | Full name |
| `GROSS_SALARY` | Number | Contract salary |
| `EARNED_SALARY` | Number | Actual earned amount |
| `DEDUCTIONS` | Number | Tax and loan deductions |
| `NET_SALARY` | Number | Final take-home pay |

*Sample rows below use randomly generated placeholder values — not real employee data.*

| SALARY_DATE | ZONE | SALARY_GROUP | DEPARTMENT | GROSS_SALARY | DEDUCTIONS | NET_SALARY |
|---|---|---|---|---|---|---|
| 2025-01-01 | Zone A | Worker | Dept 1 | 38,500 | 3,200 | 35,300 |
| 2025-01-01 | Zone B | Staff | Dept 2 | 62,000 | 5,100 | 56,900 |
| 2025-01-01 | Zone C | Executive | Dept 3 | 210,000 | 18,400 | 191,600 |

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard development |
| **Power Query (M)** | Data cleaning and transformation |
| **DAX** | Measures and calculations |
| **Microsoft Excel** | Source data format |
| **Oracle SQL** | Database management |
| **GitHub** | Version control |

---

##  Dashboard Pages

1. **Executive Summary** — company-wide KPIs and trends
2. **Statistical Analysis** — mean, standard deviation, variance
3. **Zone & Department Analysis** — geographic/organizational breakdown
4. **Monthly Analysis** — time-based trends
5. **Anomalies** — no-pay and overtime cases
6. **Employee Details** — individual drill-through
7. **Department Details** — department-level analysis
8. **Zone Summary** — zone-wise salary distribution
9. **Employee History** — individual salary trend over time
10. **Department Employee Details** — team-level performance analysis

---

##  Analytical Approach

The dashboard was designed to answer questions typically relevant to HR and Finance teams working with payroll data:

- How does average pay vary across zones, departments, and employee categories?
- Are there statistically significant outliers in salary or deduction patterns?
- What do month-over-month and year-over-year payroll trends look like?
- Which departments show unusually high overtime or payroll cost?
- Are there missing-pay or zero-salary records that need HR follow-up?
- How consistent are deduction rates over time, and are there unexplained spikes?

---

##  Data Cleaning Steps

1. Corrected column data types (dates formatted, IDs set to text).
2. Trimmed inconsistent text values (extra spaces in department names).
3. Handled null/missing values appropriately per column.
4. Removed blank and duplicate rows.
5. Added calculated columns:
   - `PAYMENT_STATUS` — flags zero-salary records
   - `OVERTIME_BONUS` — captures earned salary exceeding gross salary
   - `DEDUCTION_PERCENT` — tracks deduction proportion
   - `YEAR` / `MONTH_NAME` — enables time-based analysis

---

##  Data Model

- Built a dedicated **Date table** using DAX's `CALENDAR()` function, marked as the official Date Table to enable time-intelligence functions.
- Established relationships between the payroll fact table and supporting dimension tables (zone, department, employee category).

```
Date Table ──┐
             ├──< Payroll Fact Table >── Zone Dimension
Employee ────┘                       └── Department Dimension
```

---

## 📐 DAX Measures

<details>
<summary><b>Financial Measures</b></summary>

- Total Net Salary
- Total Gross Salary
- Total Deductions
- Average Net Salary
- Deduction Rate (%)
- Total Overtime
- Year-over-Year Growth (%)
</details>

<details>
<summary><b>Statistical Measures</b></summary>

- Mean, Standard Deviation, Variance
- Max / Min Net Salary
- Upper / Lower Bands (outlier detection)
- Upper / Lower Outlier counts
</details>

<details>
<summary><b>Operational Measures</b></summary>

- Total Employees
- No-Pay Count
- Monthly Total Net Salary
- Overall Average Line
</details>

---

##  Sample Insights 

> The examples below use placeholder numbers to demonstrate the type of insight the dashboard surfaces — not the original project's real findings.

- **Pay spread:** Standard deviation was a large share of mean salary, pointing to a wide pay range across grades — a signal for reviewing salary-band consistency.
- **Overtime hotspots:** A small number of departments accounted for a disproportionate share of overtime cost — useful for headcount planning conversations.
- **Seasonal dips:** Certain months consistently showed lower payroll totals, useful for budget forecasting.
- **Zone pay gaps:** Meaningful average-salary differences existed across zones, flagged for a pay-equity review.

---

##  Data Quality

- Verified core formula integrity (`Net = Earned − Deductions`) across the dataset.
- Checked for duplicate rows, negative salary values, and missing data.
- Documented overall data completeness as part of the QA process.

---

##  Key Skills Demonstrated

- End-to-end BI workflow: raw data → cleaning → modelling → DAX → multi-page dashboard
- Statistical analysis within a BI tool (mean, standard deviation, outlier banding)
- Time-intelligence modelling using a dedicated date table
- Anomaly detection logic (no-pay cases, deduction spikes, overtime outliers)
- Multi-level drill-through design (company → zone → department → employee)
- Working with large, real-world, imperfect datasets

---

## Author

**Muqadas Yasin**
Business Data Analytics Student — COMSATS University Islamabad

*Built during an IT Department internship, with mentorship and technical guidance from my industry supervisors.*

---

## 📄 License

MIT License — free to use with attribution. 
