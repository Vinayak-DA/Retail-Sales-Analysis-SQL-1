Retail Sales Analysis - SQL Project

📊 Overview

This project focuses on Retail Sales Analysis using SQL. The goal is to analyze transactional sales data, uncover key business insights, and answer important questions related to sales performance, customer behavior, and trends.

I have structured the dataset, cleaned and transformed data, and formulated key business questions, answering them using SQL queries.

🚀 Features

Data Cleaning & Preprocessing: Identified and handled missing values.

Exploratory Data Analysis (EDA): Basic statistics and data exploration.

Business Insights: Queries addressing real-world retail sales problems.

Aggregate Analysis: Sales trends, top customers, category-based insights.

Time-based Analysis: Monthly sales trends, best-selling periods, and customer behavior by time.

🔧 Tools & Technologies Used

SQL: Data extraction, cleaning, and analysis

PostgreSQL / MySQL: Database for executing queries

Excel: Initial dataset exploration

📂 Project Structure

📁 Retail_Sales_Analysis_SQL/
 ├── 📄 README.md  # Project documentation
 ├── 📄 sql_query_p1.sql  # SQL queries for analysis
 ├── 📂 Data/  # Retail sales dataset
 ├── 📂 Reports/  # Additional insights & visualizations

📌 Dataset Overview

The dataset contains retail sales transactions with the following attributes:

transaction_id: Unique transaction identifier

sale_date: Date of the sale

sale_time: Time of the sale

customer_id: Unique customer identifier

gender: Gender of the customer

age: Customer's age

category: Product category (e.g., Clothing, Beauty, Electronics)

quantity: Number of units sold

price_per_unit: Price per unit

cogs: Cost of goods sold

total_sale: Total sales amount

🔎 Business Questions & SQL Queries

1️⃣ Data Cleaning & Exploration

Identified missing values in key columns (transaction_id, sale_date, category, etc.)

Removed incomplete records to ensure data integrity

Counted total transactions and unique customers

2️⃣ Key Business Questions Answered

Question

SQL Query Summary

Retrieve all sales made on a specific date

WHERE sale_date = '2022-11-05'

Find all transactions where category is 'Clothing' & quantity > 4 (Nov 2022)

WHERE category = 'Clothing' AND quantity >= 4

Calculate total sales for each category

SUM(total_sale) GROUP BY category

Find the average age of customers buying 'Beauty' products

AVG(age) WHERE category = 'Beauty'

Identify transactions with total sales above 1000

WHERE total_sale > 1000

Count total transactions by gender in each category

COUNT(*) GROUP BY category, gender

Find the best-selling month each year based on average sales

RANK() OVER(PARTITION BY year ORDER BY AVG(total_sale) DESC)

Identify the top 5 customers based on highest total sales

SUM(total_sale) GROUP BY customer_id ORDER BY total_sale DESC LIMIT 5

Find unique customers per category

COUNT(DISTINCT customer_id) GROUP BY category

Categorize transactions into shifts (Morning, Afternoon, Evening)

CASE WHEN sale_time < 12 THEN 'Morning' ...

📊 Insights Gained

Top-performing categories: Identified the most popular product categories based on total sales.

Customer demographics: Found age distribution of customers purchasing specific products.

Peak sales periods: Discovered which months and times of the day had the highest sales.

High-value customers: Identified top spenders contributing the most revenue.

Gender-based purchasing behavior: Analyzed how sales vary by gender across different categories.

📌 How to Use

Load the dataset into your SQL database (PostgreSQL/MySQL).

Execute the queries in sql_query_p1.sql to analyze sales performance.


📢 Future Enhancements


Customer Segmentation: Identify customer clusters based on purchasing patterns.

Data Visualization: Create Power BI or Tableau dashboards for better insights.



-- This project demonstrates my SQL proficiency in handling real-world retail sales data. 🚀

