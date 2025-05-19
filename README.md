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
2.1 Pizza Sold by Category
- Classic pizza is the best-seller, with 15,000 units sold—outperforming all other categories.
- Supreme and Veggie pizzas follow closely, each with 12,000 units sold, indicating strong demand for both premium and vegetarian options.
- Chicken pizza ranks lowest, with 11,000 units sold, though it still maintains solid customer interest.
  Classic pizzas generated the highest revenue at $220K, underscoring their strong commercial appeal and broad customer demand.
2.2 Sales by Category 
- Classic pizzas generated the highest revenue at $220K, underscoring their strong commercial appeal and broad customer demand.
- Followed closely by Supreme pizzas, which brought in approximately $208K in revenue—despite a lower sales volume.
- Meanwhile, Chicken ($196K) and Veggie ($194K) categories maintained steady revenue performance, these categories also present opportunities for targeted growth through pricing strategies, bundling, or promotional campaigns.
2.3 Sales by Pizza Sizes
- Large pizzas dominated sales performance, generating $375K and contributing to 45.89% of total revenue.
- Medium-sized pizzas followed with $249K (30.49%), while Small pizzas brought in $178K (21.77%), reflecting consistent demand across standard size offerings.
- In contrast, Extra Large ($14K) and Double Extra Large ($1K) pizzas made minimal contributions to overall revenue. This suggests either limited market demand or a lack of visibility and promotional focus, indicating potential areas for product repositioning or strategic marketing efforts.
3.  Month-over-Month Growth by Category
- The total sales fluctuated throughout the months, with the highest growth in November 2015 (+9.95%)
- Lowest growth occurred in February 2015 (-6.64%) and December 2015 (-8.09%).
- Classic Pizza is consistently one of the top contributors in total sales. Strong growth in July (+8.97%) and November (+6.76%), but a dip in June (-7.14%).
4. Temporal Patterns
- Hourly Sales: 12 PM (Noon) is the busiest hour, generating the highest total sales. Followed closely by 1 PM and 2 PM, which together highlight the lunch-time peak (12 PM–2 PM). Another strong peak is observed around 6 PM to 8 PM, clearly corresponding to dinner-time demand.
- Weekday sales repeatedly dominate, generally comprising 70% or more of total pizza revenue.

# Recommendation
1. Seasonal Sales Strategy
- Goal: Boost low-performing months and capitalize on peak demand.
- Action: Develop a year-round marketing calendar aligned with monthly order trends.
- Tactic: Launch targeted campaigns during low-traffic periods (e.g., February and September) using seasonal themes, limited-time offers, or loyalty rewards.
- Channels: Leverage social media ads, email marketing, and influencer collaborations to reach segmented audiences with high engagement potential.
2. A/B Testing Promotions
- Goal: Determine the most effective conversion tactics.
- Action: Conduct A/B tests during off-peak months with variations in offer types (e.g., discounts, free sides, combo deals).
- Outcome: Identify which incentives yield the highest ROI and apply learnings to future campaigns.
3. Time-Based Revenue Optimization
- Goal: Maximize high-traffic lunch and dinner hours.
- Action: Offer time-specific promotions (e.g., “Lunch Combo Specials” or “Dinner Family Packs”) to increase basket size.
- Support Tools: Introduce loyalty cards or punch programs to encourage repeat purchases during those windows.
4. Product Line Repositioning
- Goal: Revitalize underperforming pizza sizes (e.g., XXL).
- Action: Improve product visibility with creative menu placement and bundled pricing.
- Tactic: Create “Group Party Bundles” featuring XXL pizzas, upsized drinks, and sides at an attractive rate to stimulate demand.
5. Weekend Revenue Boost
- Goal: Capitalize on increased weekend traffic
- Action: Launch weekend-exclusive family bundles that offer value-for-money meal deals tailored to group sizes.
- Tactic: Promote deals using geo-targeted mobile ads and in-store signage.
- 
# Conlusion 
This project highlights how data-driven analysis can uncover valuable business insights. By combining SQL for data cleaning and Power BI for visualization, this project identified key trends in sales performance, customer behavior, and product preferences. The findings reveal strong performance from Classic and Large pizzas, seasonal sales fluctuations, and peak order times during lunch and dinner hours. These insights support targeted strategies to optimize marketing, promotions, and operations. Overall, this dashboard enables smarter decision-making and demonstrates the practical impact of data analytics in a retail setting.

# Contact 
For any questions or inquiries, please contact evitanegara@gmail.com


  
