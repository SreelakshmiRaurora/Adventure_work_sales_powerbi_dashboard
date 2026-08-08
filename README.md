# Adventure Works Sales Dashboard 📊

## 📌 Project Overview

The **Adventure Works Sales Dashboard** is an interactive Power BI dashboard designed to analyze sales performance, order trends, product information, customer details, and sales territories.

The project uses Adventure Works sales data from **2020, 2021, and 2022** and demonstrates data modeling, DAX calculations, interactive filtering, and data visualization using Microsoft Power BI.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze overall sales performance.
- Track total sales, orders, and quantities.
- Calculate and monitor average order value.
- Analyze sales across different products and categories.
- Understand customer and sales-territory information.
- Identify sales trends over time.
- Build an interactive and user-friendly Power BI dashboard.
- Apply data modeling and relationships between multiple tables.

---

## 🗂️ Dataset

The project is based on the **Adventure Works** dataset.
### [Dataset link](https://www.kaggle.com/datasets/shaikhshoeb/adventureworks-dataset-for-data-analysis?utm_source=chatgpt.com)

### Sales Data

Sales data is available for:

- 2020
- 2021
- 2022

The yearly sales files were imported as CSV files and combined/used in Power BI for analysis.

### Main Tables Used

- Adventure work sales
- AdventureWorks Customer Lookup
- AdventureWorks Product Lookup
- AdventureWorks Product Categories Lookup
- AdventureWorks Product Subcategories Lookup
- AdventureWorks Calendar Lookup
- AdventureWorks Territory Lookup
- AdventureWorks Returns Data

---

## 🔗 Data Model

The project uses a relational data model connecting sales data with lookup/dimension tables.

Key relationships include:

- Sales → Customer
- Sales → Product
- Product → Product Subcategory
- Product Subcategory → Product Category
- Sales → Calendar
- Sales → Territory
- Sales → Returns

This model allows different dimensions to filter and analyze the sales data interactively.

---

## 🧮 DAX Measures

The dashboard includes the following key measures:

### Total Sales

### DAX
Sales Amount =
'Adventure work sales'[OrderQuantity] *
RELATED('AdventureWorks Product Lookup'[ProductPrice])
Total Sales =
SUM('Adventure work sales'[Sales Amount])
Total Orders =
DISTINCTCOUNT('Adventure work sales'[OrderNumber])
Total Quantity =
SUM('Adventure work sales'[OrderQuantity])
Average Order Value =
DIVIDE([Total Sales], [Total Orders])

## 📊 Key Performance Indicators

The dashboard includes four main KPI cards:

💰 Total Sales
🛒 Total Orders
📦 Total Quantity
📈 Average Order Value

These KPIs provide a quick overview of the overall sales performance.

## 📈 Dashboard Analysis

The dashboard provides analysis of:

### Sales Performance

Analyze total sales generated across the selected period.

### Order Analysis

Track the number of orders and understand order activity.

### Quantity Analysis

Analyze the total quantity of products sold.

### Average Order Value

Measure the average sales value generated per order.

### Product Analysis

Compare sales performance across products and product categories.

### Time Analysis

Analyze sales trends across different dates and years.

### Territory Analysis

Explore sales performance across different sales territories

## 🎛️ Interactive Features

The dashboard includes interactive filters/slicers for relevant business dimensions such as:

Year
Country
Product Category
Gender

Users can select different values to dynamically update the dashboard visuals.

## Dashboard preview
![Dashboard](https://github.com/SreelakshmiRaurora/Adventure_work_sales_powerbi_dashboard/blob/main/Screenshot%202026-08-08%20113417.png?raw=true)
