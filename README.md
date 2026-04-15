# 📊 Adventure Works Report (Power BI)

## 🧭 Project Overview

This project analyzes the sales performance of a bike shop over a 3-year span, with a detailed analysis of different products, the product categories they belong to, and sales across different regions using an interactive Power BI dashboard.

---

## 📚 Learning Context

This project was developed as part of the "Microsoft Power BI Desktop for Business Intelligence" course on Udemy.

The goal of the exercise was to practice:
- ETL processes
- data modeling
- building interactivity into dashboards

---

## 🖼️ Dashboard Preview

![Dashboard Screenshot](images/Screenshot_1.png)

---

## 🎯 Business Approach

Taking a look at the data from a business point of view, identifying the KPIs that are going to be used is an essential part of the project. The most important KPIs, which are displayed at the top of the main dashboard, are:

* Revenue
* Profit
* Orders
* Return Rate

This project also aims to answer key questions, such as:

* Which product is returned the most?
* Which regions generate the highest revenue?
* How does a possible price adjustment affect a product's profit?
* How do sales trend over time?
* Which customer drives the most revenue?

---

## 📁 Dataset

**Source** 

The dataset used in this project was provided in the course. It is based on the "Adventure Works" dataset, which is a free and publicly available dataset.

**Dataset Structure**

The dataset contains transaction-level sales data including:

| Column           | Description                 |
| ---------------- | --------------------------- |
| Order Date       | Date of the transaction     |
| Region           | Geographic sales region     |
| Product Category | Product classification      |
| Sales            | Total revenue generated     |
| Profit           | Profit from the transaction |
| Quantity         | Number of items sold        |

---

## 🧹 Data Cleaning & Preparation

Before building the dashboard, several preprocessing steps were performed:

* Removed duplicate records
* Handled missing values
* Standardized date formats
* Created calculated columns for time-based analysis (Year, Quarter, Month)
* Ensured consistent category naming

These steps ensured **data accuracy and reliable insights**.

---

## 🧩 Data Model

A structured data model was implemented in Power BI to optimize analysis.

Key components:

* Fact table: **Sales Transactions**
* Dimension tables:

  * Date
  * Product Category
  * Region

Relationships were created to support **time-based and categorical analysis**.

---

## 🧮 Key Measures (DAX)

Several calculated measures were created using DAX:

```DAX
Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Profit Margin = DIVIDE([Total Profit], [Total Sales])
```

These measures allow dynamic aggregation across filters and visuals.

---

## ✨ Dashboard Features

The interactive dashboard includes:

* 📈 **Sales trend analysis over time**
* 🌍 **Regional performance comparison**
* 📦 **Product category breakdown**
* 📊 **KPI indicators for sales and profit**
* 🎛️ **Interactive slicers and filters**

Users can dynamically explore data by:

* Region
* Product category
* Time period

---

## 🔍 Key Insights

Some insights identified from the analysis:

* Sales peak during **Q4**, indicating strong seasonal demand.
* The **West region consistently generates the highest revenue**.
* **Technology products contribute the largest share of profit**.
* Certain regions show **high revenue but relatively low profit margins**, suggesting pricing or cost issues.
