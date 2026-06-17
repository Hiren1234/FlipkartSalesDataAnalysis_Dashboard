# 🛒 Flipkart Sales Performance Analysis Dashboard

A comprehensive Power BI Business Intelligence dashboard designed to analyze sales performance, profitability, customer behavior, product performance, and regional trends across Flipkart's operations.

---

## 📌 Project Overview

This project provides a 360-degree view of business performance through interactive Power BI visualizations and KPI tracking. The dashboard enables stakeholders to monitor revenue, profitability, customer retention, product performance, and regional growth using dynamic filters and time-intelligence calculations.

The solution follows industry-standard Business Intelligence practices and demonstrates how data can be transformed into actionable insights for executive decision-making.

---

## 🎯 Business Objectives

The dashboard was developed to answer key business questions:

* How is overall sales performance trending?
* Which products generate the highest revenue and profit?
* Which regions contribute most to business growth?
* How effective is customer retention?
* Which customer segments drive the most revenue?
* How can management identify growth opportunities and risks?

---

## 🏗 Dashboard Architecture

The dashboard follows a Star Schema data model consisting of:

### Fact Table

**Sales**

* Total Sales
* Total Profit
* Total Orders
* Total Customers
* Profit Margin %
* Growth %
* YTD Sales
* QTD Sales
* MTD Sales
* Repeat Customers

### Dimension Tables

**Products**

* Product Name
* Category

**Customers**

* Customer Name
* Customer Segment

**Regions**

* Region

**Date**

* Year
* Month
* Quarter
* Time Intelligence Support

---

## 📊 Dashboard Pages

### 1. Executive Summary

Provides a high-level business overview using key KPIs:

* Total Sales
* Total Profit
* Total Orders
* Total Customers
* Profit Margin %

Visuals:

* KPI Cards
* Monthly Trend Analysis
* Category Revenue Breakdown

---

### 2. Sales Analysis

Focuses on revenue and profitability trends.

Visuals:

* YTD Sales
* QTD Sales
* MTD Sales
* Monthly Sales Trend
* Regional Profit Waterfall
* Profit Distribution by Region
* Sales & Profit Pivot Table

Key Outcomes:

* Identify sales trends
* Track profitability
* Compare performance across periods

---

### 3. Product Analysis

Evaluates category and product-level performance.

Visuals:

* Category Treemap
* Top Products by Profit
* Top Products by Sales
* Category Sales Distribution

Key Outcomes:

* Identify top-performing products
* Analyze category contribution
* Optimize product portfolio

---

### 4. Region Analysis

Examines geographic business performance.

Visuals:

* Sales Map
* Regional Profit Comparison
* Region Ranking Table
* Regional Growth Analysis

Key Outcomes:

* Identify growth regions
* Compare regional profitability
* Support expansion decisions

---

### 5. Customer Analysis

Provides customer intelligence and retention insights.

Visuals:

* Total Customers KPI
* Repeat Customers KPI
* Customer Segment Analysis
* Customer Ranking Table
* Customer Contribution Analysis

Key Outcomes:

* Measure retention
* Identify high-value customers
* Understand segment performance

---

### 6. Detailed Data

A detailed analytical layer for validation and ad-hoc analysis.

Contains:

* Total Sales
* Total Profit
* Total Orders
* Growth %
* Profit Margin %
* Regional Performance Metrics

Used by:

* Business Analysts
* Finance Teams
* Operations Teams
* Senior Management

---

## 📈 Key Performance Indicators (KPIs)

| KPI              | Description               |
| ---------------- | ------------------------- |
| Total Sales      | Overall revenue generated |
| Total Profit     | Net profit earned         |
| Total Orders     | Number of transactions    |
| Total Customers  | Customer base size        |
| Profit Margin %  | Profitability efficiency  |
| Growth %         | Period-over-period growth |
| YTD Sales        | Year-to-Date revenue      |
| QTD Sales        | Quarter-to-Date revenue   |
| MTD Sales        | Month-to-Date revenue     |
| Repeat Customers | Customer retention metric |

---

## 📚 DAX Measures Used

### Sales Metrics

```DAX
Total Sales = SUM(Sales[TotalSales])

Total Profit = SUM(Sales[TotalProfit])

Total Orders = SUM(Sales[TotalOrders])

Total Customers = DISTINCTCOUNT(Sales[CustomerID])
```

### Profit Margin

```DAX
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales]
)
```

### Customer Retention

```DAX
Customer Retention Rate =
DIVIDE(
    [Repeat Customers],
    [Total Customers]
)
```

### Time Intelligence

```DAX
YTD Sales =
TOTALYTD(
    [Total Sales],
    'Date'[Date]
)

QTD Sales =
TOTALQTD(
    [Total Sales],
    'Date'[Date]
)

MTD Sales =
TOTALMTD(
    [Total Sales],
    'Date'[Date]
)
```

---

## 💡 Business Insights

### Product Insights

* Identify high-profit products.
* Detect low-margin volume leaders.
* Optimize inventory planning.

### Regional Insights

* Compare profitability across regions.
* Identify emerging growth markets.
* Support marketing allocation decisions.

### Customer Insights

* Monitor customer retention.
* Analyze customer contribution.
* Prioritize high-value customer segments.

### Sales Insights

* Track monthly performance trends.
* Measure growth using time-intelligence metrics.
* Support strategic planning.

---

## 🚀 Future Enhancements

* Customer Lifetime Value (CLV)
* Product Return Rate Analysis
* Forecasting Models
* AI-Powered Insights
* YoY Growth Analysis
* Drill-Through Functionality
* Advanced Customer Segmentation

---

## 🛠 Tools & Technologies

* Microsoft Power BI
* DAX (Data Analysis Expressions)
* Power Query
* Data Modeling
* Star Schema Design
* Business Intelligence Reporting

---

## 📂 Repository Structure

```text
Flipkart-Sales-Analysis/
│
├── Dataset/
├── Dashboard Screenshots/
├── FlipkartSalesAnalysisDashboard.pbix
├── README.md
└── Documentation/
```

---

## 📷 Dashboard Preview

Add screenshots of:

* Executive Summary
* Sales Analysis
* Product Analysis
* Region Analysis
* Customer Analysis

inside the repository for visual reference.

---

## 🎯 Project Outcomes

This dashboard enables business users to:

✔ Monitor business performance in real time

✔ Analyze product profitability

✔ Identify high-growth regions

✔ Improve customer retention

✔ Support data-driven decision making

✔ Transform raw data into actionable business insights

---

### Author

**Hiren Patel**

Data Analyst | Business Intelligence Enthusiast | Power BI Developer

Focused on transforming business data into actionable insights through analytics, visualization, and storytelling.
