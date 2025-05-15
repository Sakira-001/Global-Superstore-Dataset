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
10. [Author](#author)
11. [Conclusion](#conclusion)
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
4. **Borough with Most Collisions**: Brooklyn
5. **Most Common Contributing Factor**: Driver Inattention/Distraction
6. **Peak Collision Hours**: Between 3 PM – 6 PM
7. **Collisions by Vehicle Type**:
   - Passenger Vehicles: 58%
   - Commercial Vehicles: 18%
   - Two-Wheelers (Motorcycles, Bicycles): 9%
   - Emergency Services: 3%
   - Others: 6%
   - Unknown/Not Reported: 6%
8. **Seasonal Pattern**: Highest collisions recorded in October, lowest in February
9. **Most Affected Demographic**: Motorists and pedestrians injured in Brooklyn and Queens
10. **Location Hotspots**: Most incidents occurred in densely populated areas with high traffic volume

---

## Insights & Conclusions
1. **Leading Causes of Collisions**:
   - The top contributing factor to collisions is "Unspecified", meaning a lack of detailed reporting.
   - Driver inattention/distraction is the most reported cause, emphasizing the need for awareness campaigns on focused driving.
2. **Fatalities Across Boroughs**:
   - Brooklyn has the highest fatalities among pedestrians, motorists, and cyclists.
   - Motorists experience the most fatalities overall, suggesting that driver safety improvements are needed.
3. **Vehicle Types in Collisions**:
   - Passenger vehicles account for the highest number of collisions, far exceeding any other vehicle type across all boroughs.
   - Bicycles, taxis, motorcycles, and buses contribute to accidents but at significantly lower numbers compared to passenger vehicles.
   - Brooklyn leads in overall collisions, followed by Queens and the Bronx, possibly due to higher traffic density and population.

---

## Tools & Techniques Used
1. **Power BI**:
   - Power Query Editor for extensive data cleaning and transformation.
   - DAX (Data Analysis Expressions) to calculate key metrics like total collisions, injuries, fatalities, and percentage breakdowns.
   - Slicers for dynamic filtering by borough, vehicle type, month, and contributing factors.
   - Custom Visuals including bar charts, pie charts, stacked columns, KPIs, and heatmaps for clear insight presentation.
2. **Figma**: Designed visual mockups and layout guides to ensure a clean, user-friendly dashboard interface.

---

## Questions & Answers
### Q1: Compare the % of total accidents by month. Do you notice any seasonal patterns? 
**A**: Yes, a clear seasonal pattern emerges. The highest percentage of accidents occurred in October, followed by June and August. The months with the lowest accident rates were February and January.

### Q2: Break down accident frequency by day of week and hour of day. Based on this data, when do accidents occur most frequently?
**Ans**: - Accidents peak sharply around midnight (12:00 AM) — likely due to the timestamp default or batch reporting practices — followed by a steady increase from 6:00 AM, with consistent spikes between 8:00 AM to 6:00 PM, especially around 3:00 PM to 6:00 PM, coinciding with afternoon rush hours.
         - By Day of Week: Fridays have the highest accident frequency, followed closely by Thursdays and Wednesdays.
Weekends (especially Sundays) see fewer incidents, likely due to reduced commuting traffic.

### Q3:  On which particular street were the most accidents reported? What does that represent as a % of all reported accidents? 
**Ans**: The street with the most reported accidents was Brooklyn.

### Q4: What was the most common contributing factor for the accidents reported in this sample (based on 
Vehicle 1)? What about fatal accidents specifically?  
**Ans**: - The most common contributing factor across all accidents (based on Vehicle 1) was Unspecified.
         - For fatal accidents specifically, the leading contributing factor remained Unspecified.

---

## Recommendation
1. Enhance Driver Awareness & Distraction Prevention Campaigns: Implementing stricter penalties for distracted driving and Conducting public awareness campaigns on focused driving and accident prevention.
2. Improve Traffic Control & Law Enforcement: Increase traffic patrols in high-collision areas and Enforce speed limits, right-of-way laws, and lane discipline more strictly.
3. Develop Safer Infrastructure for Cyclists & Pedestrians: Expand dedicated bike lanes and pedestrian-friendly zones and Install more traffic calming measures (e.g., speed bumps, pedestrian islands).
4. Targeted Safety Measures in High-Collision Boroughs: Brooklyn & Queens: Implement city-wide road safety programs due to high fatalities.
5. 
---

## Author
This project was created by Sakira, a data analyst with a strong background in data storytelling, dashboard design, and analytical problem-solving. I specialize in using tools like Excel, Power BI, and SQL to transform raw data into actionable insights. I'm passionate about building user-centric dashboards that reveal trends, improve decision-making, and create impact across various industries.. [[www.linkedin.com/in/sakira-daodu-b44666275](https://www.linkedin.com/in/sakira-daodu-b44666275/)].

---

## Conclusion
