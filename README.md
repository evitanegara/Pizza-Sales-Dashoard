# Business Understanding 
The Pizza Sales Dashboard project aims to analyze sales data to uncover performance trends, customer behavior, and operational insights. By leveraging data from 1 Jan 2015 to 31 Dec 2015, the dashboard enables a data-driven understanding of revenue patterns, product performance, and time-based sales behavior. The end goal is to guide strategic decision-making that enhances profitability, customer targeting, and overall business efficiency. Understanding digital sales footprints helps businesses:
- Anticipate customer needs and preferences
- Track high- and low-performing products
- Optimize promotions based on time, size, and category patterns
- Improve customer retention and satisfaction

#  Key Data Preparation Steps (SQL-Based)
1. Understanding the Data Structure
  - This data contains 48,620 rows and 12 columns.
  - Key dimensions divided by : order_date, pizza_name_id, pizza_category, pizza_size
  - Key metrics: quantity, unit_price, total_price
2. Data Cleaning in SQL Server
   - Null Checks: No null values found across critical fields
   - Duplicate Removal: Validated uniqueness of each pizza per order
   - Categorical Standardization: Unified pizza_size from short codes (S, M, L, XL) to full form (Small, Medium, Large, etc.) Ensured consistent casing and formatting in pizza_category
   - Outlier Detection: Checked for outliers in pricing (unit_price), all values were within logical range
   All SQL queries used for cleaning, aggregation, and KPI calculations are provided in a separate script file.

#  KPI and Business Objectives
1. Overall Metrics
  - Total Sales: $818,000
  - Total Pizzas Sold: 50,000
  - Total Orders: 21,000
  - Average Pizzas per Order: 2.32
2. Analytical Goals
- Track monthly sales and order volume trends
- Identify best-selling pizza categories and sizes
- Compare month-over-month category sales with growth and decline
- Visualize sales distribution by hour, day,  weekday and weekend
- Implement a dynamic calendar heatmap for granular trend analysis

  
