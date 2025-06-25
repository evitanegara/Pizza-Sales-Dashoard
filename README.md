## Pizza Sales Analysis Dashboard

## Project Background

This project analyzes a full year of pizza sales data (2015) to uncover performance trends across product categories, sizes, and customer behavior. Built in Power BI, the dashboard identifies key growth periods, optimal selling times, and product preferences to support strategic decisions in marketing, inventory, and operations for a pizza chain.

## Dataset Overview

The dataset contains transactional-level records with the following structure:

| Column           | Description                              |
|------------------|------------------------------------------|
| pizza_id         | Unique pizza identifier                  |
| order_id         | Unique order ID                          |
| pizza_name_id    | Pizza SKU/Name reference                 |
| quantity         | Number of pizzas ordered                 |
| order_date       | Date of order                            |
| order_time       | Time of order                            |
| unit_price       | Price per pizza                          |
| total_price      | Total price per order line               |
| pizza_size       | Size (Small, Medium, Large, etc.)        |
| pizza_category   | Category (Classic, Veggie, etc.)         |
| pizza_ingredients| Ingredients included                     |
| pizza_name       | Full product name                        |

Power BI was used for data modeling, KPI analysis, and interactive dashboard creation.

## Key Data Preparation Steps (SQL-Based)

1. **Understanding the Data Structure**  
   - Dataset consists of 48,620 rows and 12 columns

2. **Data Cleaning in SQL Server**
   - **Null Checks:** Verified no nulls in critical fields  
   - **Duplicate Removal:** Ensured unique pizza entries per order  
   - **Categorical Standardization:**  
     - Converted size codes (S, M, L, XL) to full text (Small, Medium, Large, Extra Large)  
     - Standardized casing in pizza_category  
   - **Outlier Detection:** Confirmed all unit_price values were within logical range  

👉 [SQL Data Prep Script](https://drive.google.com/file/d/19FBEyBPYv54wlq3db06rU1sfi1bs_ptk/view?usp=sharing)

3. **Dashboard Development:** Built interactive dashboard in Power BI with slicers, visuals, and metrics.

## Visualization 
<p align="center">
  <img src="https://github.com/user-attachments/assets/7137c99b-712c-4ed4-aa59-12a0154c593e" alt="Pizza Dashboard Page 1" width="700"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/1b0ea1d1-1c4a-4689-bb5b-8e3b77a5b8c4" alt="Pizza Dashboard Page 2" width="700"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f48f7b2d-d3ac-4433-ad54-b5c5131fb100" alt="Pizza Dashboard Page 3" width="700"/>
</p>



## Executive Summary

The pizza sales data from 2015 reveals total revenue of $818K generated from over 21,000 orders and 50,000 pizzas sold, with an average of 2.32 pizzas per order. Classic and Supreme pizzas dominate category-level sales, while Large and Medium sizes are the most preferred among customers.

Sales peaked in July, driven by strong performance in the Classic ($19.7K) and Supreme ($18.2K) categories, contributing to the highest monthly revenue of $73K. Weekday sales significantly outpaced weekend activity, with Fridays and lunch/dinner hours showing the highest demand.

---

## Insights Deep-Dive

### Monthly Sales & Order Trends

- Order volume in 2015 exhibits noticeable fluctuations. July stands out as the peak month with 1,935 total orders. Tooltip analysis shows strong category performance—particularly for Classic (962 orders) and Veggie (804 orders), driving $73K in revenue.
- In contrast, October records one of the lowest order counts at 1,646 and revenue ($64K), with significant decreases in all types of pizza sales compared to July.
- Other high-performing months include May (1,853), January (1,845), and August (1,841), indicating steady engagement during early-year and summer periods.
- A sharp decline of nearly 200 orders from August to September signals a potential demand contraction that warrants investigation.
- Despite the variation in order volume, monthly revenue remains relatively stable (ranging from $64K to $73K).
![image](https://github.com/user-attachments/assets/7890b8d5-f916-49b0-9f8f-47ea45f2b722)
![image](https://github.com/user-attachments/assets/c6211cf3-0d7c-47ce-b395-d3d96207cbee)




### Key Product Performance by Category and Size

- Classic pizzas lead with $220K in total sales, driven by Medium ($61K), Small ($70K), and Large ($75K) sizes.
- Supreme pizzas follow at $208K, with top sales from Large ($94K) and Medium ($66K) sizes.
- Chicken pizzas total $196K, with the Small size at $28K and Large as the highest at $102K.
- Veggie pizzas reach $194K, with Large ($104K), Medium ($57K), and Small ($32K) contributing steadily.
- Extra Large and Double Extra Large sizes remain marginal across all categories.
  ![image](https://github.com/user-attachments/assets/7ae5560e-e0f6-465b-9af6-d9acc1881eca)


### Sales by Pizza Size

- Large pizzas lead in revenue with $375K, showing strong customer preference for group-friendly sizes and better value-per-slice.
- Medium pizzas follow at $249K, indicating consistent demand among small groups and individuals.
- Small pizzas generate $178K, suggesting a steady niche driven by solo diners or portion-conscious customers.
- Extra Large pizzas contribute just $14K, while Double Extra Large pizzas show negligible sales—highlighting low customer interest in oversized options.
  ![image](https://github.com/user-attachments/assets/17547c89-e1b1-46eb-9e63-708847540ae7)


### Monthly Sales Spike Analysis – July 2015

- July 2015 recorded the highest total sales of the year, reaching $72.6K, a strong +6.34% increase from June’s $68.2K.
- All four pizza categories saw sales increases, led by:
  - Veggie pizzas: Jumped by +10.46% ($16.0K → $17.7K)
  - Classic pizzas: Rose by +8.97% ($18.0K → $19.6K)
  - Chicken pizzas: Saw a modest rise of +5.69% ($16.1K → $17.0K)
  - Supreme pizzas: Minimal growth at +0.66% ($18.1K → $18.2K)
    ![image](https://github.com/user-attachments/assets/8c05be8f-9716-41cf-8116-6dd247981a8d)
    ![image](https://github.com/user-attachments/assets/df9cc190-9f15-46d3-976d-32591454db57)


### Daily and Weekly Sales Trends

- July 4 recorded the highest single-day sales at $3,864 from 105 orders, followed by notable spikes on July 3, 17, and 24.
- These dates consistently exceed the average daily sales of $2,341, indicating sharp demand surges.
- Weekends contributed only $18K (25%) of total sales, while weekdays drove $55K (75%), underlining a weekday-dominant sales pattern.
  ![image](https://github.com/user-attachments/assets/5dd3ead5-f80d-4eea-bd04-549068e9f488)
  ![image](https://github.com/user-attachments/assets/01c862ec-e2b2-4b71-97a0-b8d40323c226)



### Sales Patterns by Day of Week and Hour

- Weekday sales dominated July, contributing 75% ($55K) of total revenue, with Fridays leading at $14K, followed by Thursdays ($12K) and Wednesdays ($11K).
- Weekends accounted for only 25% ($18K), with Saturday ($10K) slightly ahead of Sunday and Tuesday (both $8K).
- Hourly performance reveals two distinct demand peaks:
  - Lunch hours (~1 PM / 13:00) mark the strongest sales spike with $10,151, the highest across all hours
  - Dinner hours (17:00–19:00) also see elevated sales, ranging from $7K to $8.2K
- Late-night hours (after 21:00) and early openings (10:00–11:00) show minimal activity, together contributing less than 5% of daily sales
![image](https://github.com/user-attachments/assets/bf12724e-d63e-40d0-b99b-c779792f2661)
![image](https://github.com/user-attachments/assets/67edc83c-cb5f-45a1-a065-9ff16cc6520e)


---

## Recommendations

### Sales Trend Optimization

- **Seasonal Promotions:** Reinforce marketing efforts during low-performing months (e.g., September–October) by:
  - Launching targeted ads for past buyers and lookalike audiences
  - Collaborating with food influencers on Instagram, TikTok, and YouTube
  - Running email marketing campaigns with festive themes and exclusive discounts
  - Leveraging seasonal messaging to create urgency and boost interest
- **Flash Deals During Peak Hours:** Capitalize on demand spikes at 13:00 (lunch) and 17:00–19:00 (dinner) with time-limited discounts or combo deals.
- **Friday-Focused Offers:** Launch new products or value bundles on Fridays—the top sales day—to maximize visibility and conversion.

### Menu & Product Strategy

- **Bundle High-Demand Sizes:** Promote Large and Medium pizzas in family combos or "Buy One Get One" campaigns.
- **Rationalize Oversized Options:** Review performance of Extra Large and Double Extra Large pizzas; reduce stock or repackage for parties.
- **Promote Veggie Options:** Support the growing Veggie segment through health-conscious or eco-themed campaigns like "Meatless Mondays."

### Customer Engagement

- **Launch Weekly Offers:** Introduce midweek promotions (e.g., "Two-Topping Tuesdays" or free drink with pizza) to boost slow weekdays.
- **Loyalty Programs:** Encourage repeat orders with pizza points, tier-based discounts, or birthday rewards.

### Operational Planning

- **Improve Inventory Forecasting:** Use daily/hourly sales patterns to plan dough and ingredient prep, minimizing overstock and waste.
- **Optimize Labor Scheduling:** Align staff shifts with peak demand hours to ensure fast service and reduce downtime.



  
