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

# Executive Summary & Insights
1. Monthly Sales Performance
- The monthly trend shows fluctuations in customer orders throughout the year 2015, with visible peaks and troughs that reflect changes in customer demand, seasonal influences, and potentially marketing or operational activity.
- July (1,935 orders) emerged as the highest-performing month, likely driven by summer holidays, family gatherings, or effective marketing campaigns.
- This was followed closely by May (1,853 orders), January (1,845), and August (1,841)—indicating strong customer engagement in the first half of the year and during late summer.
- In contrast, October (1,646) and September (1,661) marked the lowest points in order volume. This downturn may be linked to post-summer spending slowdowns, back-to-school season, or reduced promotional activity.
- In addition, there was a sharp decline of 180 orders from August to September, representing a significant drop in demand that warrants further investigation.
2. Category and Size Analysis
- Top-Selling Category: Classic (15K pizzas)
- High Revenue Sizes: Large (46% of total revenue), followed by Medium and Small
- Underperformer: Double Extra Large XXL had minimal sales despite higher price point
3.  Month-over-Month Growth by Category
- The total sales fluctuated throughout the months, with the highest growth in November 2015 (+9.95%)
- Lowest growth occurred in February 2015 (-6.64%) and December 2015 (-8.09%).
- Classic Pizza is consistently one of the top contributors in total sales. Strong growth in July (+8.97%) and November (+6.76%), but a dip in June (-7.14%).
4. Temporal Patterns
- Hourly Sales: 12 PM (Noon) is the busiest hour, generating the highest total sales. Followed closely by 1 PM and 2 PM, which together highlight the lunch-time peak (12 PM–2 PM). Another strong peak is observed around 6 PM to 8 PM, clearly corresponding to dinner-time demand.
- Weekday sales repeatedly dominate, generally comprising 70% or more of total pizza revenue.
  
