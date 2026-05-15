Maven Market Performance Dashboard
📊 Project Overview
This project features a comprehensive Power BI Dashboard developed to analyze the performance of Maven Market, a fictional multi-national grocery chain. The dashboard provides a high-level "Topline Performance" view for executives, allowing them to track key metrics across different regions, timeframes, and product categories.

The primary goal of this report is to transform raw transactional data into actionable insights regarding revenue trends, regional performance, and progress against business targets.

🚀 Key Features
Topline Performance Tracking: A dedicated page for high-level KPIs including Total Revenue, Total Profit, and Transaction Volume.

Geospatial Analysis: Map-based visuals to identify high-performing regions (e.g., Portland sales analysis).

Temporal Trends: "Weekly Revenue Trending" charts to monitor growth and seasonality.

Target Monitoring: Gauge and KPI visuals (Revenue vs. Target) to measure success against predefined business goals.

Interactive Slicers: Advanced filtering by region, product, and date for granular data exploration.

🗃️ Data Model
The report utilizes a Star Schema data model for optimized performance and scalability:

Fact Table: Transactions (containing sales, quantities, and dates).

Dimension Tables:

Customers: Demographic data and loyalty information.

Products: Details on product brands, categories, and pricing.

Stores: Store locations and types.

Regions: Geographical hierarchy (Country, State, City).

Calendar: A dedicated date table for Time Intelligence calculations.

💡 Key DAX Measures
The dashboard leverages several custom DAX measures to drive the visualizations:

Total Revenue: SUMX(Transactions, Transactions[quantity] * Related(Products[product_price]))

Total Profit: [Total Revenue] - [Total Cost]

Revenue vs. Target: A comparison measure used in gauges to visualize performance gaps.

Weekly Revenue: Time-intelligence calculation to aggregate sales on a weekly grain.

🛠️ Tools Used
Power BI Desktop: For data modeling, DAX development, and report design.

Power Query (M): Used for data cleaning, ETL processes, and merging disparate data sources.

DAX (Data Analysis Expressions): For advanced analytical calculations and KPIs.  
![Dashboard Preview](Screenshot 2026-05-15 161633.png)
