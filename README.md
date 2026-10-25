# 📊 SQL Data Analytics Project

## 📌 Project Overview

This project is an end-to-end **SQL Data Analytics project** focused on exploring and analyzing sales data using **Microsoft SQL Server**.

The project covers both **Exploratory Data Analysis (EDA)** and **Advanced Data Analytics**, transforming raw sales data into meaningful business insights about **customers, products, sales performance, and trends**.

The main goal of this project was to strengthen my practical SQL skills by working with a real-world-style dataset and applying different analytical techniques to answer business questions.

---

## 🎯 Project Objectives

The analysis focuses on:

- Exploring the database structure and understanding the available data.
- Analyzing key business metrics such as sales, orders, customers, and products.
- Identifying sales trends and changes over time.
- Evaluating product and customer performance.
- Performing cumulative and running-total analysis.
- Comparing performance across different periods.
- Analyzing part-to-whole relationships.
- Segmenting customers and products based on business metrics.
- Building comprehensive **Customer** and **Product** reports.

---

## 🛠️ Tools & Technologies

- **Microsoft SQL Server**
- **SQL Server Management Studio (SSMS)**
- **SQL**
- **Git & GitHub**

---

## 📂 Project Structure

```text
sql-data-analytics-project/
│
├── datasets/
│   └── DataWarehouseAnalytics.bak
│
├── docs/
│   └── Project Roadmap
│
├── scripts/
│   ├── 01_database_exploration.sql
│   ├── 02_dimensions_exploration.sql
│   ├── 03_date_range_exploration.sql
│   ├── 04_measures_exploration.sql
│   ├── 05_magnitude_analysis.sql
│   ├── 06_ranking_analysis.sql
│   ├── 07_change_over_time_analysis.sql
│   ├── 08_cumulative_analysis.sql
│   ├── 09_performance_analysis.sql
│   ├── 10_data_segmentation.sql
│   ├── 11_part_to_whole_analysis.sql
│   ├── 12_report_customers.sql
│   └── 13_report_products.sql
│
└── README.md
```

---

# 🔍 Part 1: Exploratory Data Analysis (EDA)

The first part of the project focuses on understanding the database and discovering the main characteristics of the data.

## 1. Database Exploration

Exploring the database structure, tables, columns, and relationships to understand how the data is organized.

## 2. Dimensions Exploration

Analyzing categorical dimensions such as:

- Customers
- Products
- Countries
- Categories
- Subcategories

This helps understand the different groups available for analysis.

## 3. Date Range Exploration

Analyzing the available date ranges to understand:

- First and last order dates
- Historical coverage of the dataset
- Customer age ranges

## 4. Measures Exploration

Calculating important business metrics such as:

- Total Sales
- Total Quantity Sold
- Average Selling Price
- Total Orders
- Total Products
- Total Customers

## 5. Magnitude Analysis

Comparing measures across different dimensions to understand where business activity is concentrated.

Examples include:

- Customers by country
- Customers by gender
- Products by category
- Revenue by category
- Revenue by customer
- Distribution of sold items across countries

## 6. Ranking Analysis

Identifying top and bottom performers using SQL ranking techniques.

Examples:

- Top-performing products
- Lowest-performing products
- Top customers by revenue
- Customers with the highest number of orders

---

# 📈 Part 2: Advanced Data Analytics

The second part goes beyond basic exploration and focuses on deeper analytical techniques.

## 7. Change Over Time Analysis

Analyzing how business performance changes over time.

This includes:

- Sales trends by year
- Sales trends by month
- Customer growth
- Quantity trends
- Time-based aggregation

These analyses help identify growth patterns, seasonality, and changes in business performance.

---

## 8. Cumulative Analysis

Using SQL window functions to calculate cumulative metrics such as:

- Running Total Sales
- Moving Average Price

This helps track business performance progressively over time.

---

## 9. Performance Analysis

Comparing current performance with historical benchmarks.

Techniques include:

- Year-over-Year analysis
- Previous-period comparisons
- Average performance comparison
- Product performance evaluation

This helps determine whether products are performing **above or below previous periods and historical averages**.

---

## 10. Data Segmentation

Grouping data into meaningful business segments.

### Product Segmentation

Products are grouped into cost ranges to analyze how products are distributed across different price segments.

### Customer Segmentation

Customers are classified based on their **spending behavior and relationship with the business**.

Example segments include:

- VIP Customers
- Regular Customers
- New Customers

This makes it easier to understand different customer groups and their contribution to the business.

---

## 11. Part-to-Whole Analysis

Analyzing how individual categories contribute to overall business performance.

For example:

- Revenue contribution by product category
- Percentage of total sales generated by each category

This helps identify which categories have the greatest impact on overall revenue.

---

# 📊 Business Reports

The final stage of the project combines multiple analytical techniques into two comprehensive SQL reports.

## 👥 Customer Report

The Customer Report provides a consolidated view of customer behavior and performance.

It includes metrics such as:

- Total Orders
- Total Sales
- Total Quantity Purchased
- Total Products Purchased
- Customer Lifespan
- Recency
- Average Order Value
- Average Monthly Spend

Customers are also segmented based on their purchasing behavior.

---

## 📦 Product Report

The Product Report provides a consolidated view of product performance.

It includes:

- Total Orders
- Total Sales
- Total Quantity Sold
- Total Customers
- Product Lifespan
- Recency
- Average Order Revenue
- Average Monthly Revenue

Products are also segmented based on their revenue performance.

---

# 🧠 SQL Skills Applied

Throughout this project, I practiced and applied:

- `SELECT`
- `WHERE`
- `GROUP BY`
- `ORDER BY`
- Aggregate Functions
- `CASE WHEN`
- Date Functions
- CTEs
- Subqueries
- Window Functions
- `RANK()`
- `ROW_NUMBER()`
- `LAG()`
- `SUM() OVER()`
- Running Totals
- Moving Averages
- Data Segmentation
- Time-Series Analysis
- Part-to-Whole Analysis
- KPI Calculation
- Business Reporting

---

# 💡 Key Takeaways

This project helped me improve my ability to move beyond simply writing SQL queries and start using SQL as a **data analysis tool**.

I gained practical experience in:

- Understanding and exploring unfamiliar datasets.
- Translating business questions into SQL queries.
- Selecting the right metrics for different analytical problems.
- Using window functions for advanced analysis.
- Analyzing trends and performance over time.
- Segmenting customers and products.
- Building reusable SQL reports for business analysis.


---

## 👤 About Me

I'm **Ahmed Badour**, a Computer Science student interested in **Data Analysis, Business Intelligence, and Data Engineering**.

I enjoy transforming raw data into meaningful insights and building practical data projects using technologies such as:

- SQL
- Excel
- Power BI
- Python

### 🔗 Connect With Me

**GitHub:**  
https://github.com/Ahmedbadour14

---

⭐ If you found this project useful, feel free to explore the repository and check out my other data projects.
