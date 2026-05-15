# HR Analytics Power BI Dashboard

## Project Overview

This project is an interactive **HR Analytics Dashboard** built using **Microsoft Power BI**.  
The dashboard helps analyze employee data and provides useful insights related to employee attrition, salary distribution, gender ratio, department-wise employee count, job roles, age groups, and overall workforce performance.

The main goal of this project is to help HR teams understand employee trends and make better data-driven decisions.

---

## Business Problem

HR teams need to monitor employee details, attrition trends, salary patterns, and department-wise workforce distribution.  
Without a proper dashboard, it becomes difficult to identify important HR issues such as high attrition, salary imbalance, and workforce gaps.

This Power BI dashboard solves this problem by providing a clear and interactive view of HR data.

---

## Objective

The objective of this project is to:

- Analyze total employee count
- Identify attrition trends
- Compare male and female employee distribution
- Analyze salary by job role and department
- Understand age group distribution
- Find top paid job roles
- Help HR teams make data-driven decisions

---

## Dataset

The dataset used in this project contains HR employee information such as:

- Employee ID
- Employee Name
- Gender
- Age
- Department
- Job Role
- Salary
- Date of Joining
- Attrition
- Experience
- Education Field

> Dataset File: `hr-data-analysis (1).xlsx`

---

## Tools Used

- **Microsoft Power BI**
- **Power Query**
- **DAX**
- **Microsoft Excel**
- **GitHub**

---

## KPIs Used

The dashboard includes the following key performance indicators:

- Total Employees
- Active Employees
- Attrition Count
- Attrition Rate
- Average Age
- Average Salary
- Male Employees
- Female Employees
- Department-wise Employees
- Job Role-wise Salary

---

## Dashboard Features

- Interactive KPI cards
- Department-wise employee analysis
- Gender-wise employee count
- Age group analysis
- Salary distribution
- Job role-wise salary analysis
- Attrition analysis
- Slicers and filters for better interactivity
- Clean and user-friendly dashboard design

---
## DAX Measures Used 
Total Employees = DISTINCTCOUNT(data[Emp ID])

Total Male Employees =
CALCULATE(
    DISTINCTCOUNT(data[Emp ID]),
    data[Gender] = "Male"
)

Total Female Employees =
CALCULATE(
    DISTINCTCOUNT(data[Emp ID]),
    data[Gender] = "Female"
)

Average Age =
ROUND(AVERAGE(data[Age]), 0)
