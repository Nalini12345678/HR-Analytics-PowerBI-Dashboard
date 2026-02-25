# HR Analytics & Employee Attrition Dashboard

## 📊 Project Overview

This project analyzes employee workforce data to identify attrition patterns, salary distribution, hiring trends, and employee performance insights using Power BI.

The dashboard helps HR managers understand workforce behavior and make data-driven decisions.

## 🎯 Business Objective

- Identify attrition rate
- Analyze overtime impact on attrition
- Compare salary vs attrition
- Monitor hiring and exit trends
- Track workforce growth
- Department-level performance analysis

## 📁 Dataset Information

- 1000 Employee Records
- 7 Departments
- Salary variation based on experience
- 20% Attrition Rate
- Hire & Exit Dates
- Overtime, Education, Performance Rating
- City & Marital Status

## 📈 Key KPIs

- Total Employees
- Active Employees
- Employees Left
- Attrition Rate %
- Average Salary
- Average Tenure
- Hiring Trend
- Exit Trend
- Net Headcount Growth

## 🧮 Important DAX Measures

Attrition Rate %:
DIVIDE([Employees Left], [Total Employees])

Employees Left:
CALCULATE(COUNT(HRData[EmployeeID]), HRData[Attrition] = "Yes")

Tenure:
IF(HRData[Attrition] = "Yes",
   DATEDIFF(HRData[HireDate], HRData[ExitDate], YEAR),
   DATEDIFF(HRData[HireDate], TODAY(), YEAR)
)

## 📊 Dashboard Pages

1. Executive Summary
2. Attrition Deep Dive
3. Hiring & Exit Trend Analysis

## 🛠 Tools Used

- Power BI
- DAX
- Excel
- Data Modeling

## 💼 Resume Description

Developed an HR Analytics Dashboard in Power BI to analyze employee attrition, salary trends, and workforce growth using advanced DAX and business intelligence techniques.
