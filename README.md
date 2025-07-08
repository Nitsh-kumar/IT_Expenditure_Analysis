# 💼 IT Expenditure Analysis Dashboard – Power BI

This Power BI project focuses on analyzing IT expenditures across regions, business areas, and cost categories. It provides actionable insights into actual vs. forecasted vs. planned IT spend, identifies budget misalignments, and highlights cost trends and overspending departments.

---

## 📊 Objective

- Understand how IT costs are distributed across regions, functions, and cost elements.
- Analyze variances between actual, forecast, and plan expenditures.
- Identify cost drivers such as labor and shared services.
- Enable business-level drill-down to locate inefficient spending.

---

## 📁 Dataset Overview

- **Region, Country, Business Area**
- **IT Area, IT Sub Area, Cost Element Group**
- **Actual, Forecast, and Plan Expenditures**
- **Monthly Aggregation**

---

## 🛠️ Key Features

- Cleaned and standardized Excel data
- DAX measures for variance, cumulative spend, and KPI insights
- Date formatting and field categorization for slicers
- Fully interactive visual dashboards

---

## 📐 Dashboards & Visuals

### 🔹 1. IT Spend Analysis

Includes KPI cards and comparisons of actual vs. forecasted spend by region and time.

![IT Spend Analysis](./f61d13c3-1688-4afd-b9a1-d1ed96887f05.png)

---

### 🔹 2. Cost Variance Analysis

Tracks how much each business area deviates from its plan and forecasts.

![Cost Variance Analysis](./95fc30fc-628f-4b9a-ac15-01ef625412d0.png)

---

### 🔹 3. Business Area Drilldown

Visualizes actual IT spend across countries and business units with a tree map and bar charts.

![Business Area Drill Down](./7ec6407d-b7f0-4617-880c-da3d9512434a.png)

---

## 📌 DAX Highlights

```dax
Total Actual = SUM('IT Expenditure dataset'[Actual])
Variance Actual vs Plan = [Total Actual] - [Total Plan]
Variance % Actual vs Plan = DIVIDE([Variance Actual vs Plan], [Total Plan], 0)
