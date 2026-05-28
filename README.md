# 🤖 AI Job Market Intelligence Dashboard

A comprehensive Power BI dashboard analyzing global 
AI job market trends, salary benchmarks and remote 
work patterns across 30,000 records from 20 countries.

## 🎯 Project Overview

| Property | Details |
|---|---|
| Tool | Power BI Desktop |
| Dataset | Kaggle — Global AI Job Market 2024-2025 |
| Records | 30,000 rows (2 datasets combined) |
| Countries | 20 |
| DAX Measures | 20 |
| Visuals | 4 |

## 🔧 Technical Details

### Power Query
- Loaded and appended 2 datasets into 30,000 row master table
- Decoded coded values (EN→Entry Level, FT→Full-Time)
- Added custom columns (Remote Category, Salary Band)
- Built Star Schema using Reference tables
- Created Date Dimension table using M code

### Data Model — Star Schema
Fact_Jobs (30,000 rows)
├── Dim_Job
├── Dim_Company
├── Dim_Employee
└── Dim_Date

### DAX Measures (20 total)
- Core KPIs: Total Jobs, Avg Salary, Median Salary
- Ranking: RANKX with DENSE and ALLSELECTED
- Time Intelligence: DATESYTD, DATEADD
- Dynamic Titles: SELECTEDVALUE

## 💡 Key Insights

- **$128,226 gap** between Executive and Entry Level salary
- **Remote Premium:** Remote jobs pay $1,356 more than On-Site
- **Switzerland** pays 2.7x more than India for same AI roles
- **Perfect 33% split** across Remote, Hybrid and On-Site
