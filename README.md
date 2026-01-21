# Zepto Database Analysis (PostgreSQL)

Project Overview
This project performs an end-to-end SQL-based data analysis on Zepto product inventory data. The objective is to clean raw data, analyze pricing and discount patterns, evaluate stock availability, and generate business insights using PostgreSQL. This project is created as a portfolio project to demonstrate practical SQL and data analysis skills.

Tools & Technologies
PostgreSQL, pgAdmin 4, SQL, Git, GitHub, Windows OS

Dataset Description
The dataset contains product-level information from Zepto, including product name, category, MRP, discounted selling price, discount percentage, available quantity, stock status, and product weight.
Dataset file used: zepto_v2.csv

Database Schema
Table name: zepto
Columns:
category (VARCHAR)
name (VARCHAR)
mrp (NUMERIC)
discountPercent (NUMERIC)
availableQuantity (INTEGER)
discountedSellingPrice (NUMERIC)
weightInGms (INTEGER)
outOfStock (BOOLEAN)
quantity (INTEGER)

Data Cleaning Steps
Checked for null values across all columns
Identified invalid pricing records where MRP was zero
Converted pricing values from paise to rupees
Verified stock availability values
Ensured consistency between pricing, quantity, and availability fields

SQL Analysis Performed
Counted total number of products in the dataset
Identified distinct product categories
Analyzed in-stock vs out-of-stock products
Detected duplicate product names with multiple SKUs
Found top 10 products with the highest discount percentage
Identified high-MRP products that are out of stock
Calculated estimated revenue per product category
Analyzed products with high MRP and low discount
Identified top categories based on average discount percentage
Calculated price per gram to identify best-value products
Grouped products into Low, Medium, and Bulk weight categories
Calculated total inventory weight per category

Key Insights
Certain categories generate higher revenue despite moderate discounts
High-MRP products tend to go out of stock more frequently
Bulk-weight products provide better value per gram
Discount patterns vary significantly across categories

Repository Structure
Zepto_data_analysis folder contains:
   zepto_data_analysis.sql file with all SQL queries
   zepto_v2.csv dataset file
README.md project documentation file

Future Enhancements
Add indexes to improve query performance
Use CTEs and window functions for advanced SQL analysis
Connect PostgreSQL with Python for data visualization
Create dashboards using Power BI or Tableau

Author
Sarmistha Naskar
Aspiring Data Analyst

Acknowledgment
This project is created for learning and portfolio purposes to demonstrate SQL-based data analysis skills.
