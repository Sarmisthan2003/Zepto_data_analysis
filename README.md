# 🛒 Zepto Database Analysis (PostgreSQL)

📌 PROJECT OVERVIEW
This project presents an end-to-end SQL-based data analysis on Zepto product inventory data using PostgreSQL.  
The goal is to clean raw data, analyze pricing and discount patterns, evaluate stock availability, and derive meaningful business insights.  
This is a portfolio-focused project designed to showcase strong SQL and data analysis skills.

────────────────────────────────────────
🛠️ TOOLS & TECHNOLOGIES

🐘 PostgreSQL  
🧰 pgAdmin 4  
🧾 SQL  
🌐 Git & GitHub  
💻 Windows OS  

────────────────────────────────────────
📂 DATASET DESCRIPTION

The dataset contains product-level information from Zepto including product name, category, MRP, discounted selling price, discount percentage, available quantity, stock status, and product weight.  
📄 Dataset file used: zepto_v2.csv

────────────────────────────────────────
🗄️ DATABASE DESIGN

A relational table named `zepto` was created with the following fields:  
category, product name, MRP, discount percentage, available quantity, discounted selling price, weight in grams, out-of-stock flag, and quantity.

────────────────────────────────────────
🧹 DATA CLEANING

✔ Checked for NULL values across all columns  
✔ Identified and handled invalid pricing records (MRP = 0)  
✔ Converted pricing values from paise to rupees  
✔ Verified stock availability indicators  
✔ Ensured data consistency across quantity and pricing fields  

────────────────────────────────────────
📊 SQL ANALYSIS

• Counted total products  
• Identified distinct product categories  
• Analyzed in-stock vs out-of-stock products  
• Detected duplicate product names 
• Found top 10 products with highest discount percentages  
• Identified high-MRP products that are out of stock  
• Calculated estimated revenue per category  
• Analyzed products with high MRP but low discounts  
• Identified top categories by average discount  
• Calculated price per gram to find best-value products  
• Grouped products by weight (Low / Medium / Bulk)  
• Calculated total inventory weight per category  

────────────────────────────────────────
📈 KEY INSIGHTS

📊 Certain categories generate high revenue despite moderate discounts  
🚫 High-MRP products tend to go out of stock more frequently  
⚖️ Bulk-weight products provide better value per gram  
🔍 Discount patterns vary significantly across categories  

────────────────────────────────────────
📁 REPOSITORY CONTENTS

📄 zepto_data_analysis.sql – SQL queries used for analysis  
📄 zepto_v2.csv – Dataset file  
📄 README.md – Project documentation  

────────────────────────────────────────
🚀 FUTURE ENHANCEMENTS

⚡ Add indexes to improve query performance  
🧠 Use CTEs and window functions for advanced SQL analysis  
📈 Connect PostgreSQL with Python for visualization  
📊 Build dashboards using Power BI or Tableau  

────────────────────────────────────────
👤 AUTHOR

**Sarmistha Naskar**  
🎯 Aspiring Data Analyst  
