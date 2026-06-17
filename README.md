## 📊 HR Attrition Analysis Dashboard


---

## 🔷 Project Overview:

-  This project presents an interactive HR Attrition Analysis Dashboard built in Microsoft Excel using Power Pivot, DAX Measures, Pivot Tables, Pivot Charts, and Slicers.

-  The dashboard helps analyze employee attrition trends, workforce performance, employee experience, and overtime patterns across departments, enabling HR professionals to make data-driven decisions.


---

## 🔷 Business Problem:

-  Employee attrition can significantly impact organizational productivity, employee morale, and recruitment costs.

-  This dashboard aims to answer key HR questions:

    - Which departments experience the highest attrition?
    - What is the employee exit rate by gender?
    - How does overtime relate to employee attrition?
    - How does employee experience affect employee exit?
    - How do employee performance and experience vary across departments?
    - What workforce trends can HR monitor using interactive filters?


---

## 🔷 Tools & Technologies:

-  Microsoft Excel
-  Power Pivot
-  DAX (Data Analysis Expressions)
-  Pivot Tables
-  Pivot Charts
-  Slicers
-  Data Modeling


---

## 🔷 Dataset Overview:

-  The project uses an HR Attrition dataset organized across 5 tables:

  - Fact_Attrition   :–  Employee attrition, overtime, tenure, and workforce-related data.
  - Dim_Employee     :–  Employee details.
  - Dim_Date         :–  Date information used for analysis.
  - Dim_Performance  :–  Employee performance ratings.
  - Dim_Satisfaction :–  Employee satisfaction and engagement metrics.


- Dataset Link :- https://docs.google.com/spreadsheets/d/19OnZjrlF-U2tP-OD7CRajCiLKBn8EP4Y/edit?gid=61728937#gid=61728937


---

## 🔷 Analytics Workflow:

```text
Raw Data
    ↓
Data Cleaning
    ↓
Data Modeling
    ↓
Calculated Columns
    ↓
DAX Measures
    ↓
Pivot Tables & Charts
    ↓
Interactive Dashboard
```

## 🔷 DATA MODEL

-  The project follows a Power Pivot data model connecting employee, performance, satisfaction, date, and attrition data.

![Data Model](Images/data_model.png)

---

## 🔷 Calculated Columns

- Custom calculated columns were created to enhance analysis and reporting.

1. Month(1)
-  Created in Dim_Date_1 table
-  Created to clean and standardize it as the original “month” field contained full date values instead of month names

2. Attrition_Count
-  Created in Fact_Attrition table
-  Converted Attrition_satisfaction column values into binary format (1 = Yes, 0 = No) to calculate total attrition easily in pivot tables and visuals.

3. Experience_Score
-  Created in Dim_Satisfaction table
-  Calculated as the average of four experience-related factors per employee to create a single score used for overall experience analysis through DAX measures

![Calculated Columns](Images/calculated_columns.png)

---

## 🔷 DAX Measures

- Several DAX measures were created to support dynamic KPI calculations.

- Examples:

    - Current Employees
    - Attrition Count
    - Attrition Rate
    - Overtime Rate
    - Average Experience Score
    - Average Performance Rating

![DAX Measures](Images/DAX_Measures.png)

---

## 🔷 KPI Summary

- The dashboard includes dynamic KPI cards that respond to slicer selections.

- ### KPIs

    -  Current Employees
    -  Attrition Rate
    -  Avg Experience Score
    -  Overtime %
    -  Avg Performance

![KPI Creation](Images/KPI_Creation.png)

---

## 🔷 Dashboard Preview

![HR Dashboard](Images/Dashboard.png)

---

## 🔷 Interactive Features

- ### Filters

    - Department
    - Gender

- ### Visualizations

- Employees Lost by Department
- Attrition by Gender
- Attrition & Overtime by Department
- Performance Rating & Employee Tenure by Department
- Employee Experience Analysis by Department

All visuals and KPI cards update dynamically based on slicer selections.

---

## 🔷 Key Insights

- Research & Development experienced the highest employee attrition.
- Departments with higher overtime levels showed greater attrition tendencies.
- Employee experience scores varied across departments.
- Performance ratings remained relatively consistent across departments.
- Gender-based attrition patterns can be analyzed dynamically using slicers.

---

## 🔷 Dashboard Demo

- A short dashboard walkthrough demonstrating KPI and chart interactivity is available below.

- **Demo:** `Videos/Dashboard_Demo.gif`

---

## 🔷 Interactive Dashboard

- Download and explore the dashboard locally:

- **Dashboard Workbook:** [HR_Attrition_Dashboard.xlsx](Dashboard/HR_Attrition_Dashboard.xlsx)

---

## 🔷 Repository Structure

```text
HR-Attrition-Dashboard/
│
├── Dataset/
│   └── hr_attrition_raw.xlsx
│
├── Dashboard/
│   └── HR_Attrition_Dashboard.xlsx
│
├── Images/
│   ├── Dashboard.png
│   ├── Data_Model.png
│   ├── Calculated_Columns.png
│   ├── DAX_Measures.png
│   └── KPI_Creation.png
│
├── Videos/
│   └── Dashboard_Demo.gif
│
└── README.md
```

---

## 🔷 Skills Demonstrated

- Data Cleaning
- Data Modeling
- Power Pivot
- DAX Calculations
- KPI Development
- Dashboard Design
- HR Analytics
- Data Visualization
- Business Insight Generation


---

## 🔷 Author

**Ekta Singh Chauhan**

Aspiring Data Analyst

Focused on building projects in:

- Excel
- SQL
- Python
- Power BI
- Data Analytics

---

