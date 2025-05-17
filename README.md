# Global-Superstore-Dataset
Global Superstore is a global online retailer based in New York, boasting a broad product catalog and  aiming to be a one-stop-shop for its customers. Global The superstore’s clientele, hailing from 147  different countries, can browse through an endless offering with more than 10,000 products.
---

## Table of Contents
1. [Overview](#overview)
2. [Raw Data](#raw-data)
3. [Dashboard & Dashboard Features](#dashboard-features)
4. [Data Cleaning Process](Data--cleaning--process&preprocessing)
5. [Key Metrics](#key-metrics)
6. [Insights & Conclusions](#insights--conclusions)
7. [Tools & Techniques Used](#tools--techniques-used)
8. [Questions & Answers](#questions--answers)
9. [Recommendation](#Recommendation)
10. [Conclusion](#conclusion)
11. [Author](#author)
---

## Overview
This interactive Power BI dashboard provides a comprehensive overview of the company's sales and profit performance across multiple regions and product categories. The dashboard is designed to support data-driven decision-making by visualizing key metrics, uncovering trends, and identifying high-performing areas.

---

## Raw Data
The raw data for this dashboard includes a comprehensive dataset of the Global Superstore Dataset. It consists of the following fields:

1. **Row ID**
2. **Order ID**
3. **Order Date**
4. **Ship Date**
5. **Ship Mode**
6. **Customer ID**
7. **Customer Name**
8. **Segment**
9. **City**
10. **State**
11. **Country**
12. **Postal Code**
13. **Market**
14. **Region**
15. **Product ID**
16. **Category**
17. **Sub-Category**
18. **Product Name**
19. **Sales**
20. **Quantity**
21. **Profit**
22. **Category**
23. **Shipping Cost**
24. **Order Proximity**

---

### Data Cleaning Process in Power Query
- **Removed Duplicates**: Duplicate records were identified and removed in the Customer ID column to prevent double-counting.
- **Handling Missing Values**: Blank or null fields in key columns were replacing with appropriate values (e.g., Profit, Product Name, Country).
- **Find and Replace**: Used the Find and Replace to fill in missing values in some columns.

---

## Dashboard Features
- **Interactive Filters**: Users can filter the dashboard by year, country, category, and sub-category, enabling targeted exploration of profit, sales, shipping cost, and discount trends across different regions and product types.
- **Visualizations**: The dashboard integrates bar charts, column charts, and KPI cards to visually communicate top-performing countries, product profitability, shipping costs, and regional comparisons.
- **Profit and Product Analysis**: Separate visuals highlight the most and least profitable products, top-selling items by country, and product subcategories with high shipping costs, helping identify what drives or drains profit in various markets.
- **Location-Based Insights**: Detailed comparisons between cities (e.g., Lafayette vs. Lancaster) and countries (e.g., U.S. vs. Nigeria) reveal regional variations in shipping costs, discount impact, and sales patterns.
- **Discount Impact Analysis**: The dashboard explores how discount levels influence profitability, especially contrasting markets like Nigeria and the U.S., offering insights into promotional effectiveness.
- **Highlight Cards (KPIs)**: Key metrics such as Total Sales, Total Profit, Total Shipping Cost, and Average Discount are displayed prominently at the top to provide a quick summary of business performance.
- **User-Friendly Design**: A clean layout with consistent fonts, colors, and intuitive slicers ensures ease of navigation and interpretation for both analysts and non-technical users.
- **Responsive Insights**: All visual elements are fully interactive and update in real-time based on user filter selections, allowing dynamic, scenario-based analysis.

![Global_Superstore_DASHBOARD]("")

---

## Key Metrics
1. **Total Sales**: $2,297,201
2. **Total Profit**: $286,400
3. **Total Shipping Cost**: $64,068
4. **Average Discount**: 15%
5. **Top 3 Countries by Total Profit (2014)**:
   - United States
   - India
   - China
6. **Top 3 Best-Selling Products by Profit**:
   - Canon imageCLASS 2200 Advanced Copier
   - Sharp AL-1530CS Digital Copier
   - Hoover WindTunnel Plus Vacuum
7. **Top Subcategories with Highest Shipping Costs**:
   - Chairs
   - Bookcases
   - Tables

---

## Insights & Conclusions
1. **High Discounts Do Not Guarantee High Profits**:
   - Cities like Lancaster and other regions with high discount rates still underperformed in profit, indicating that excessive discounting may be reducing overall profitability.
2. **U.S. Leads in Sales and Profit but Incurs Highest Shipping Costs**:
   - The U.S. remains the top market for both sales and profit; however, it also has the highest shipping costs, which could reduce profit margins if not optimized.
3. **Specific Product Subcategories Contribute to Losses in Certain Regions**:
   - Subcategories such as Tables, Bookcases, and Machines consistently perform poorly in Southeast Asia, pointing to issues with market fit or pricing.
4. **Home Office Segment Shows Strong Performance Across Multiple Regions**:
   - The Home Office customer segment shows steady growth in sales and profit, suggesting a stable and potentially scalable target audience for marketing and product development.   
---

## Tools & Techniques Used
1. **Power BI**:
   - Power Query Editor for extensive data cleaning and transformation.
   - DAX (Data Analysis Expressions) to calculate key metrics.
   - Slicers for dynamic filtering.
   - Custom Visuals including bar charts, pie charts, stacked columns, and KPIs for clear insight presentation.
2. **Figma**: Designed visual mockups and layout guides to ensure a clean, user-friendly dashboard interface.

---

## Questions & Answers
### Q1a: What are the three countries that generated the highest total profit for Global Superstore in 2014?  
**Ans**: United States, India and China
### Q1b:  For each of these three countries, find the three products with the highest total profit. Specifically, what are the products’ names and the total profit for each product?   
**Ans**: - United States(Canon imageCLASS, Hewlett-Packard (Hewlett ...), GBC Document (GBC Do...))
         - India(Sauder Classic Bookcase (Sauder Cla...), Cisco Smart Business (Cisco Sma...), Hamilton Beach Blender (Hamilton...) – $1.4K)
         - China(Sauder Bookcase (Sauder...) – $1.5K, Bush Classic Furniture (Bush Cl...), HP Copier (HP Cop...))

### Q2: Identify the 3 subcategories with the highest average shipping cost in the United States. 
**Ans**: Tables, Bookcases and Chair

### Q3a:  Assess Nigeria’s profitability (i.e., total profit) for 2014. How does it compare to other African countries? 
**Ans**: Total Profit: -$5,959.27. This is the worst-performing country in Africa in terms of profit.
### Q3b:  What factors might be responsible for Nigeria’s poor performance? You might want to investigate shipping costs and the average discount as potential root causes.
**Ans**: - Products in Nigeria are often sold at significant discounts, 
impacting profit margins.
         - Nigeria has one of the highest average shipping costs among African countries.

### Q4a: Identify the product subcategory that is the least profitable in Southeast Asia. Note: For this question, assume that Southeast Asia comprises Cambodia, Indonesia, Malaysia, Myanmar (Burma), the Philippines, Singapore, Thailand, and Vietnam.  
**Ans**: Tables
### Q4b: Is there a specific country i n Southeast Asia where Global Superstore should stop offering the subcategory identified in 4a?  
**Ans**: Myanmar (Burma) had the lowest profit from Tables and may not be a viable market for this subcategory.

### Q5a: Which city is the least profitable (in terms of average profit) in the United States? For this analysis, discard the cities with less than 10 Orders. b) Why is this city’s average profit so low? 
**Ans**:Philadelphia
### Q5b: Why is this city’s average profit so low? 
**Ans**: - High Discount Rates and Frequent Returns were observed.
         - The city also had low average order value, affecting profit margins.

### Q6: Which product subcategory has the highest average profit in Australia?  
**Ans**: Copier

### Q7: Who are the most valuable customers and what do they purchase? 
- **Ans**: - Sean Miller (United States) – Primarily purchases Copiers and Phones
         - Neel Sharma (India) – High-volume orders of Binders and Furnishings
         - Victoria Ashbrook (Australia) – Repeatedly purchases Chairs and Office Supplies
---

## Recommendation
1. Analyze discount effectiveness and reduce excessive discounting that doesn’t lead to higher profits. Emphasize value and unique selling propositions instead.
2. Review supply chain logistics in the U.S. to identify areas for cost reduction without affecting delivery times or customer satisfaction.
3. Consider retiring, bundling, or repackaging poorly performing products like Tables and Machines in Southeast Asia to avoid recurring losses.

---

## Conclusion
- This analysis provided valuable insights into the sales performance across different regions, customer segments, and product categories. While the United States remains the strongest market in terms of revenue and profit, high shipping costs and over-discounting present areas for improvement. Identifying underperforming subcategories and optimizing pricing strategies can help increase profitability globally. By focusing on high-performing segments like the Home Office category and refining regional product strategies, the company can enhance overall market efficiency and drive sustainable growth.
---

## Author
This project was created by Sakira, a data analyst with a strong background in data storytelling, dashboard design, and analytical problem-solving. I specialize in using tools like Excel, Power BI, and SQL to transform raw data into actionable insights. I'm passionate about building user-centric dashboards that reveal trends, improve decision-making, and create impact across various industries.. [[www.linkedin.com/in/sakira-daodu-b44666275](https://www.linkedin.com/in/sakira-daodu-b44666275/)].
