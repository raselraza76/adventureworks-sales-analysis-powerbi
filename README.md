# 🚴‍♂️ AdventureWorks Sales & Performance Analytics | Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Analytics-yellow)
![DAX](https://img.shields.io/badge/DAX-Advanced%20Calculations-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green)
![Data Analytics](https://img.shields.io/badge/Data%20Analytics-Business%20Intelligence-orange)

---

## 📌 Executive Summary

This project presents an interactive **sales and performance analytics solution built with Microsoft Power BI** using AdventureWorks sales data.

The solution transforms raw transactional data into an interactive business intelligence dashboard designed to monitor **revenue performance, order trends, customer demographics, product performance, regional sales, profitability, and product returns**.

The dashboard provides both **executive-level KPIs** and detailed analytical views, enabling users to identify key revenue drivers, understand customer behavior, evaluate product performance, monitor trends, and identify return-related business risks.

---

## 🎯 Project Objectives

The primary objectives of this project are to:

- Analyze overall sales and order performance
- Identify the major revenue-generating product categories
- Understand customer demographics and purchasing behavior
- Compare sales performance across countries and territories
- Analyze sales trends over time
- Evaluate product and subcategory profitability
- Monitor product return volume and return rates
- Build interactive dashboards for business decision-making
- Convert raw transactional data into actionable business insights

---

## ❓ Business Questions

This dashboard was designed to answer key business questions such as:

1. What is the overall sales and order performance?
2. Which product categories generate the most revenue?
3. Which countries contribute the highest sales?
4. How are sales changing month-over-month and year-over-year?
5. Which customer demographics represent the most valuable segments?
6. Which products and subcategories perform best?
7. What is the overall profit margin?
8. Which categories have the highest return rates?
9. Which products contribute significantly to return volume?
10. How does return performance vary across regions?

---

# 🛠️ Tech Stack & Methods

### Business Intelligence
- **Microsoft Power BI Desktop**

### Data Transformation & ETL
- **Power Query**
- Data cleaning
- Data type transformation
- Column optimization
- Data preparation
- Query transformation
- ETL workflow

### Calculations & Analytics
- **DAX (Data Analysis Expressions)**
- Calculated measures
- Time-intelligence calculations
- KPI calculations
- Percentage calculations
- Growth analysis
- Return-rate calculations

### Data Modeling
- **Star Schema**
- Fact and Dimension table relationships
- Date/Calendar dimension
- One-to-many relationships
- Relationship optimization

### Visualization
- KPI Cards
- Line Charts
- Bar Charts
- Column Charts
- Slicers
- Interactive filters
- Trend analysis
- Geographic analysis
- Drill-down analysis

---

## 📸 Dashboard Preview

![Home Dashboard](https://raw.githubusercontent.com/raselraza76/adventureworks-sales-analysis-powerbi/main/ecommerce.jpeg)


# 🗂️ Data Architecture

The analytical model follows a **Star Schema** approach.

### Fact Tables

- Sales
- Returns

### Dimension Tables

- Customers
- Products
- Territories
- Calendar

This structure helps separate transactional data from descriptive attributes and supports efficient analytical reporting.

```text
                    ┌───────────────┐
                    │   Customers   │
                    └───────┬───────┘
                            │
                            │
┌──────────────┐      ┌─────▼──────┐      ┌───────────────┐
│   Products   │──────│   Sales    │──────│  Territories  │
└──────────────┘      └─────┬──────┘      └───────────────┘
                            │
                            │
                    ┌───────▼───────┐
                    │    Calendar   │
                    └───────────────┘

                    ┌───────────────┐
                    │    Returns    │
                    └───────────────┘
