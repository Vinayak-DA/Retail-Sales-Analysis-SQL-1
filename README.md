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

sale_date: **Date of the sale**

sale_time: **Time of the sale**

customer_id: **Unique customer identifier**

gender: **Gender of the customer**

age: **Customer's age**

category: **Product category (e.g., Clothing, Beauty, Electronics)
**
quantity: **Number of units sold**

price_per_unit: **Price per unit**

cogs: **Cost of goods sold**

total_sale: **Total sales amount**

🔎 Business Questions which are answered seperatlty in SQL file

1️⃣ Data Cleaning & Exploration

Identified missing values in key columns (transaction_id, sale_date, category, etc.)

Removed incomplete records to ensure data integrity

Counted total transactions and unique customers

2️⃣ Key Business Questions Answered

-- Q.1 Write a SQL query to retrieve all columns for sales made on '2022-11-05'

-- Q.2 Write a SQL query to retrieve all transactions where the category is 'Clothing' and the quantity sold is more than 10 in the month of Nov-2022.

-- Q.3 Write a SQL query to calculate each category's total sales (total_sale).

-- Q.4 Write a SQL query to find the average age of customers who purchased items from the 'Beauty' category.

-- Q.5 Write a SQL query to find all transactions where the total_sale exceeds 1000.

-- Q.6 Write a SQL query to find the total number of transactions (transaction_id) made by each gender in each category..

-- Q.7 Write a SQL query to calculate the average sale for each month. Find out best selling month in each year.

-- Q.8 Write a SQL query to find the top 5 customers based on the highest total sales.

-- Q.9 Write a SQL query to find the number of unique customers who purchased items from each category.

-- Q.10 Write a SQL query to create each shift and number of orders (Example Morning <=12, Afternoon Between 12 & 17, Evening >17).

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

