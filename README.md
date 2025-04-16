# online_sales_data

📊 MySQL Sales Data Analysis Project
MySQL
GitHub
Data Analysis

A comprehensive MySQL-based analysis of e-commerce sales data from January to August 2024, uncovering key business insights through SQL queries. Here I'm giving breif introduction about what I have done. If you want all qurrey output and screenshot visit file .

📌 Table of Contents
Project Overview

Dataset

SQL Analysis

Key Findings
 
Visualizations

Business Recommendations

License

🔍 Project Overview
This project demonstrates my SQL skills by analyzing:

Monthly revenue trends

Product category performance

Regional sales distribution

Payment method preferences

Perfect for showcasing data analysis and SQL querying abilities to potential employers.

📂 Dataset
File: cleaned_online_sales_data.csv
Records: 240 transactions (Jan-Aug 2024)
Columns:

Transaction details (ID, date)

Product info (category, name, price)

Sales metrics (units sold, revenue)

Customer info (region, payment method)

💻 SQL Analysis
Core Queries
sql
Copy
-- Monthly Revenue & Transaction Volume
SELECT 
    EXTRACT(YEAR_MONTH FROM date) AS year_month,
    SUM(total_revenue) AS revenue,
    COUNT(DISTINCT transaction_id) AS transactions
FROM sales_data
GROUP BY year_month
ORDER BY year_month;
sql
Copy
-- Top 5 Product Categories by Revenue
SELECT 
    product_category,
    ROUND(SUM(total_revenue),2) AS category_revenue
FROM sales_data
GROUP BY product_category
ORDER BY category_revenue DESC
LIMIT 5;
View all queries

📊 Key Findings
Revenue Trends
Month	Revenue	Growth Rate
Jan	$12,540	-
Feb	$14,210	+13.3%
Mar	$15,890	+11.8%
Top Categories
Electronics ($42,150)

Home Appliances ($28,740)

Clothing ($18,920)

Regional Performance
Region Pie Chart

🚀 How to Use
Clone repository

bash
Copy
git clone https://github.com/Abhishek6290/online_sales_data.git
Import dataset to MySQL

Execute queries from queries/ folder

💡 Business Recommendations
🚀 Boost electronics promotions during high-growth months

💳 Optimize credit card checkout flow (most popular payment method)

🌏 Expand Asian market presence (emerging growth region)



📜 License
MIT License - Feel free to use and modify for your own projects.

📬 Contact
LinkedIn https://www.linkedin.com/in/abhishek-verma-52603a313/
Email abhisehkverma6290@gmail.com



