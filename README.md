# 📊 Data Analysis with SQL – Sales Intelligence Project

An end-to-end data analysis project using advanced SQL queries to uncover key business insights from a retail sales database. The project covers everything from KPIs and sales trends to customer segmentation and product performance.

## 📝 Project Overview

This SQL-based project demonstrates how structured queries can turn raw sales data into powerful insights that help guide decision-making. Using a relational data warehouse structure (fact and dimension tables), the project analyzes customer demographics, product performance, category sales, customer segments, order trends, and much more.

## 🧾 Dataset Overview

- *Source*: Simulated enterprise retail database (Star Schema format)
- *Schema Name*: gold
- *Timeframe*: Multi-year sales data (with date, quantity, and pricing metrics)

### 🧱 Data Model Structure

| Table Name          | Type       | Description |
|---------------------|------------|-------------|
| gold.fact_sales   | Fact Table | Contains sales transactions with order_number, sales_amount, quantity, product_key, customer_key, and order_date |
| gold.dim_customers| Dimension  | Customer info including customer_key, name, gender, birthdate, and country |
| gold.dim_products | Dimension  | Product info including product_key, product_name, category, subcategory, and cost |

## ⚙ Tools & Technologies

- 🐘 *SQL (T-SQL / PostgreSQL style)* – Core querying and logic
- 🧠 *Window Functions* – For advanced calculations and flexible rankings
- 📊 *Data Aggregation & Segmentation* – Using GROUP BY, CASE, JOIN, CTE, VIEW, RANK, DATE functions
- 📁 *Canva* – For visual presentation of results and insights

## 🔍 Key Business Insights Extracted

- *📈 Total Revenue*: Calculated by category, subcategory, and customer
- *🛒 Top 5 & Bottom 5 Products*: Based on total revenue
- *🧍 Customer Segments*: VIP, Regular, and New (based on lifetime value & lifespan)
- *🌍 Country-Level Stats*: Number of customers and order distribution by geography
- *👕 Product Segments*: Based on cost and average selling price
- *📆 Time-Series Trends*: Monthly & yearly trends in revenue, quantity sold, and customer count
- *📦 Product Performance Views*: Includes avg_order_revenue, monthly_sales, and segment classification (Low, Mid, High Performer)

## 🧠 Methodology Summary

The analysis was conducted through the following structured SQL approach:

1. *Schema Understanding* – Inspected metadata and data types via INFORMATION_SCHEMA
2. *KPI Calculation* – Total revenue, orders, quantity, AOV, average price
3. *Segmentation Analysis* – Customer lifetime value (LTV), cost ranges, country-level analysis
4. *Window Functions* – To rank top products and track year-over-year changes
5. *Views Created*:
   - gold.report_customers: LTV, AOV, Recency, Segment
   - gold.report_products: Sales tiers, lifespan, performance metrics

## 📽 Presentation Deck

🎞 View the visual summary of this project via Canva:  
🔗 [Click here to view the Canva Presentation](https://www.canva.com/design/DAGswhukOjA/bcGSoU3euYzKV_tAUh2mFw/view?utm_content=DAGswhukOjA&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h3b68fd60bd)
