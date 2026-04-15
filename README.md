# 📊 Adventure Works Dashboard (Power BI)

## 🧭 Project Overview

This project analyzes sales performance across different regions, product categories, and time periods using an interactive Power BI dashboard.

The objective is to transform raw sales data into **actionable business insights** through data modeling, visualization, and interactive analytics.

---

## 🎯 Business Problem

Businesses often struggle to quickly identify which products, regions, and time periods drive revenue and profitability.

This project aims to answer key questions such as:

* Which regions generate the highest revenue?
* Which product categories contribute the most profit?
* How do sales trends evolve over time?
* Are there seasonal patterns affecting performance?

---

## 📁 Dataset

**Source:** Public dataset / simulated business data

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

## 🖼️ Dashboard Preview

![Dashboard Screenshot](images/dashboard_preview.png)

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

---

## 🗂️ Repository Structure

project-folder
│
├── dashboard.pbix
├── data/
│   └── sales_data.csv
├── images/
│   └── dashboard_preview.png
└── README.md

---

## ▶️ How to Use

1. Download the `.pbix` file.
2. Open it with **Power BI Desktop**.
3. If necessary, reconnect the dataset located in the `data` folder.

---

## 🚀 Future Improvements

Potential extensions for this project include:

* Adding **customer segmentation analysis**
* Implementing **sales forecasting models**
* Incorporating additional datasets for deeper analysis
* Enhancing dashboard interactivity

---

## 👤 Author

**[Your Name]**
Data Analyst

If you found this project interesting, feel free to explore the repository or connect with me.
