Task 9 – Superstore Star Schema ⭐

Overview
Implemented a Star Schema for the Global Superstore dataset using PostgreSQL.
The dataset contains sales, customers, products, regions, and orders.

Goal: Transform raw data into dimension tables and a fact table for efficient analytics.
Star Schema

Dimensions:
dim_customer – customer details (customer_key, customer_id, customer_name, segment)
dim_product – product details (product_key, product_id, product_name, category, sub_category)
dim_location – location details (location_key, region, country, state, city, market)
dim_date – order dates (date_key, order_date, year, weeknum)

Fact Table:
fact_sales – sales transactions linked to dimensions (sales_key, customer_key, product_key, location_key, date_key, sales, profit, quantity, discount, shipping_cost, record_count)
Diagram: See star_schema_diagram.png

Queries Implemented
Total Sales by Region – identifies high-performing regions
Profit by Category – finds most profitable product categories
Data Quality Checks – row counts, null foreign keys, duplicates

Files Included
task9_star_schema_full.sql – SQL script
star_schema_diagram.png – schema diagram
task9_total_sales_by_region.csv – output CSV
task9_profit_by_category.csv – output CSV
README.md – this file
