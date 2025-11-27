# Vendor Performance Analysis – Retail Inventory & Sales
Analyzing vendor efficiency and profitability to support strategic purchasing and inventory decisions using SQL and Python

## Business Problem Statement
Vendors purchase products from us and resell them in their markets. Effective inventory and sales management are critical for optimizing profitability in this industry. Our company needs to ensure that we are not incurring losses due to inefficient pricing, poor inventory turnover, or vendor dependency.
The goal of this analysis is to:
- Bring together messy, real-world data into a single relational framework
- Analyze pricing behaviour, vendor patterns, profitability, and product movement
- Recommend business-level pricing and commercial improvements

## Executive Summary of the Insights
**_Insights and related recommendations for the way forward have been added to the uploaded summary file_**
- Our wholesale pricing strategy is not differentiated. **"Discount" has become the baseline**, and isn't a lever or an incentive for vendors.
-**Profitability does not correlate with either vendors’ purchase behaviours or sales volume**, indicating that even encouraging vendors to "buy more" within the existing pricing framework may not reap proportionate results.
- In terms of high-ticket partnerships with vendors, currently, the **revenue model  depends on many small vendors**.

## Dataset
- Multiple CSV files located in /data/ folder (sales, vendors, inventory, purchase price references, actual purchase transactions)
- Summary table created from ingested data and used for analysis

## Tools and Technologies
- SQL (Common Table Expressions, Joins, Filtering)
- Python (Pandas, Matplotlib, Seaborn)
- GitHub

## Problem-Solving Approach

- **Understanding the data across the 8 tables**

- **Data Loading:** ingestion into an SQLite database using Python and SQLAlchemy for efficient querying.

- **Data Cleaning and Reloading the clean files:**
  - Fixed inconsistent date formats using string engineering
  - Standardized text fields (Brand, Vendor Name, City)
  - Handled missing data using rules and domain logic
  - Removed duplicates and identified anomalies

- **Data Integration:** Joins across Vendor, Product, Brand, Purchase & Sales enabled unified insight extraction.

- **Feature Engineering:** These new variables power the business insights. Created metrics such as:
  - % Price Difference: Purchase Price – Actual Market Price
  - Profit Margin: Gross Profit ÷ Sales
  - Stock Turnover: Sales Quantity ÷ Purchase Quantity


## Learnings from this project
- **End-to-End ETL (Extract, Transform, Load):** Built a full ETL workflow, extracting raw CSV files, cleaning and transforming them, and loading structured data into a relational database.
  
- **Wholesale vs Retail Pricing Dynamics:** Learned how pricing, discounts, markups, freight, and taxes flow through a wholesale-to-retail business model and how they affect final profitability.
  
- **SQL for Aggregation & Performance Optimization:** Used SQL CTEs, GROUP BY aggregation, and filtering to optimize large transformations before loading into Pandas.
 
## Author & Contact
Kunika Verma

Aspiring Business Intelligence and Data Analyst

📧 Email: vermakunika01@gmail.com

🔗 [LinkedIn](https://www.linkedin.com/in/kunikaverma/)


