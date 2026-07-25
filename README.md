# Payroll Analytics Dashboard
## Crescent Textile Mills — 2021 to 2026

---

## Company Overview

Crescent Textile Mills is one of Pakistan's leading textile manufacturers operating across 10 zones with 269 departments. This dashboard analyzes 5 years of employee payroll data to drive informed decision-making across HR, Finance, and Management teams.

---

## Project Overview

This Power BI dashboard transforms 253,010 rows of raw payroll data into actionable intelligence. Built during an AI/ML internship at ITSimplera Solutions, it provides multi-level analysis from company-wide trends down to individual employee salary history.

---

## Quick Facts

| Metric | Value |
|--------|-------|
| Total Records | 253,010 rows |
| Time Period | 2021 - 2026 |
| Unique Employees | 11,864 |
| Total Zones | 10 |
| Total Departments | 269 |
| Salary Groups | 7 |
| Monthly Pay Periods | 65 months |
| Total Payroll (5 years) | 8.5 Billion PKR |

---

## Dataset Description

- File: AI_PAYROLL_DATA.csv
- Size: 13.6 MB
- Records: 253,010 rows
- Columns: 10

| Column | Type | Description |
|--------|------|-------------|
| SALARY_DATE | Date | Monthly payroll date |
| ZONE | Text | Factory zone code |
| SALARY_GROUP | Text | Employee category |
| DEPARTMENT | Text | Department name |
| EMPLOYEE_CODE | Text | Unique employee ID |
| EMPLOYEE_NAME | Text | Full name |
| GROSS_SALARY | Number | Contract salary |
| EARNED_SALARY | Number | Actual earned amount |
| DEDUCTIONS | Number | Tax and loan deductions |
| NET_SALARY | Number | Final take-home pay |

---

## Tools and Technologies

| Tool | Purpose |
|------|---------|
| Power BI Desktop | Dashboard development |
| Power Query M Language | Data cleaning and transformation |
| DAX | Measures and calculations |
| Microsoft Excel | Source data format |
| Oracle SQL | Database management |
| GitHub | Version control |

---

## Dashboard Pages

1. Executive Summary — Company-wide KPIs and trends
2. Statistical Analysis — Mean, Standard Deviation, Variance
3. Zone and Department Analysis — Geographic breakdown
4. Monthly Analysis — Time-based trends
5. Anomalies — No pay and overtime cases
6. Employee Details — Individual drill-through
7. Department Details — Department-level analysis
8. Zone Summary — Zone-wise salary distribution
9. Employee History — Employee performance tracking
10. Department Employee Details — Team performance analysis

---

## Quantitative Insights

### Payroll Overview

| Metric | Value |
|--------|-------|
| Total Net Salary (5 years) | 8.5 Billion PKR |
| Total Gross Salary (5 years) | 9.8 Billion PKR |
| Total Deductions (5 years) | 989 Million PKR |
| Average Deduction Rate | 8 to 10 percent |
| Average Net Salary | 33,618 PKR per month |
| Maximum Net Salary | 764,000 PKR |
| Minimum Net Salary | 41 PKR |

### Workforce Distribution

| Salary Group | Percentage |
|-------------|------------|
| Workers | 35.9 percent |
| Unconsolidated Workers | 33.35 percent |
| Staff | 16.08 percent |
| Hattar Employees | 8.94 percent |
| Executives | 4.34 percent |
| Managerial | 1.39 percent |

### Zone Salary Analysis

| Zone | Average Net Salary |
|------|-------------------|
| YG Zone | 161,000 PKR |
| MK Zone | 130,000 PKR |
| FN Zone | 112,000 PKR |
| SP Zone | 20,000 PKR |

### Department Analysis

| Department | Total Net Salary |
|-----------|-----------------|
| Ring U1 | 400 Million PKR |
| Ring U6 | 330 Million PKR |
| Back Process U1 | 300 Million PKR |

### Time-based Insights

| Metric | Value |
|--------|-------|
| Payroll Peak | 2025 — 181 Million PKR |
| Payroll Low Month | June — 31.4 Million PKR |
| Worst Drop | July 2023 — 58 Million PKR |
| Year-on-Year Growth | 8 to 12 percent annually |

### Anomaly Detection

| Anomaly | Count |
|---------|-------|
| No Pay Cases | 741 records |
| Overtime Cases | 16,049 rows |
| Deduction Spike 2023 | 55 percent |
| Deduction Spike 2025 | 57 percent |
| Missing Values | 18 rows |

### Statistical Analysis

| Metric | Value |
|--------|-------|
| Mean Net Salary | 33,618 PKR |
| Standard Deviation | 27,970 PKR |
| Variance | 833.45 Million |
| StdDev to Mean Ratio | 83 percent |
| Upper Band | 61,588 PKR |
| Lower Band | 5,648 PKR |

---

## Key Findings

### Finding 1 — High Pay Inequality

Standard deviation is 83 percent of the mean salary. Daily wagers earn approximately 10,000 PKR while executives earn up to 764,000 PKR. The gap ratio is 76 times between minimum and maximum salary. Salary bands per grade should be defined to address this inequality.

### Finding 2 — Ring U1 Overtime Crisis

Ring U1 has the highest payroll cost at 400 Million PKR and the highest overtime cost at 1.3 Million PKR. This dual pressure indicates understaffing, excessive production pressure, and potential employee burnout risk. A headcount review for Ring U1 is recommended.

### Finding 3 — 2023 Payroll Anomaly

Payroll dropped from 148 Million to 58 Million in July 2023, a 60 percent sudden decline. Possible causes include mass no-pay leaves, major retrenchment, or a system data entry error. HR and Finance teams should investigate this period.

### Finding 4 — Zone Pay Gap

YG Zone average salary is 161,000 PKR while SP Zone average is 20,000 PKR, representing an 8 times difference between zones. A pay equity audit is needed to ensure fair compensation across all zones.

### Finding 5 — Deduction Spikes

Normal deduction rate is 8 to 10 percent. Spikes of 55 percent in 2023 and 57 percent in 2025 are abnormal. Possible causes include bulk loan recoveries, policy changes, or audit-related deductions. Finance team investigation is required.

### Finding 6 — 741 No Pay Cases

741 employees received zero salary in at least one month. This pattern may indicate unauthorized absences, resignation processes, or disciplinary actions. HR follow-up is required for all identified cases.

---

## Recommendations

### For Finance Team

1. Investigate the 2023 and 2025 deduction spikes immediately.
2. Set an automated alert when deduction rate exceeds 15 percent.
3. Monitor monthly payroll against the 134 Million PKR baseline average.
4. Use the 8 to 12 percent annual growth trend for next year budget forecasting.

### For HR Team

1. Review all 741 no-pay employee cases and document reasons.
2. Conduct a pay equity audit across all 10 zones.
3. Define salary bands per grade to reduce the 83 percent standard deviation inequality.
4. Investigate Ring U1 overtime and consider additional hiring.
5. Track monthly headcount changes to identify attrition signals early.

### For Management and CEO

1. Ring U1 cost review is needed as it leads in both salary and overtime costs.
2. YG and MK zones justify higher pay due to skilled workforce — maintain current levels.
3. SP Zone low salary may increase attrition risk — review compensation structure.
4. The 5-year upward trend confirms payroll budget should grow 10 percent annually.
5. June consistently shows the lowest payroll — plan for seasonal operational dips.

---

## Data Quality Report

| Metric | Value |
|--------|-------|
| Total Records | 253,010 |
| Duplicate Rows | 0 |
| Negative Salaries | 0 |
| Formula Verified | NET equals EARNED minus DEDUCTIONS |
| Missing Values | 18 rows (0.007 percent) |
| Data Completeness | 99.993 percent |
| Date Range | January 2021 to May 2026 |

---

## Data Cleaning Steps

1. SALARY_DATE column type changed to Date format.
2. EMPLOYEE_CODE changed to Text type as it is an identifier not a numeric value.
3. DEPARTMENT names trimmed to remove extra spaces.
4. Null DEDUCTIONS values replaced with zero.
5. Blank rows removed from dataset.
6. Calculated columns added:
   - PAYMENT_STATUS — identifies zero salary employees
   - OVERTIME_BONUS — captures earned salary exceeding gross salary
   - DEDUCTION_PERCENT — tracks deduction proportion
   - YEAR and MONTH_NAME — enables time-based analysis

---

## Date Table

Created using DAX CALENDAR function covering January 2021 to May 2026 with the following columns:

- Date
- Year
- Month
- MonthNum — used for Jan to Dec sorting

Table marked as official Date Table in Power BI to enable time intelligence functions.

---

## DAX Measures

### Financial Measures
- Total Net Salary
- Total Gross Salary
- Total Deductions
- Average Net Salary
- Deduction Rate Percent
- Total Overtime
- YoY Growth Percent

### Statistical Measures
- Mean Net Salary
- Standard Deviation Net Salary
- Variance Net Salary
- Max Net Salary
- Min Net Salary excluding zero
- Upper Band
- Lower Band
- Upper Outliers
- Lower Outliers

### Operational Measures
- Total Employees
- No Pay Count
- Monthly Total Net
- Overall Average Line

---

## Project Structure
