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
- **Removed Duplicates**: Identified and removed duplicate rows based on Collision ID to ensure each collision record is unique.
- **Time Data Type**: Changed the time data type from Time & Date to Time only.
- **Null**: Chabged the Null values in the Borough, Steet Name and Contributing factor column to "Unknown or "Unspecified".
- **Find and Replace**: Used the Find and Replace to reduce the contents "Vehicle" and "Contributing Factors" columns.

---

## Dashboard Features
- **Interactive Filters**: Users can slice and explore the data by borough, vehicle type, contributing factors, month, and injury/fatality type for flexible, in-depth analysis.
- **Visualizations**: The dashboard incorporates bar charts, pie charts, stacked columns, and heat maps to clearly display accident trends, contributing causes, and spatial distribution.
- **Custom Groupings**: Vehicle types and contributing factors were grouped into meaningful categories (e.g., Passenger, Commercial, Unknown) to simplify interpretation.
- **Time-Based Analysis**: Monthly and hourly trend graphs allow users to detect seasonal patterns and peak collision times.
- **Highlight Cards (KPIs)**: Summary cards show total collisions, injuries, and fatalities, providing an instant snapshot of the overall impact.
- **User-Centric Design**: Custom color schemes, consistent font styles, and intuitive slicer layouts were applied to ensure clarity, readability, and visual appeal.
- **Responsive Insights**: All charts dynamically update based on selected filters, helping users draw targeted conclusions based on specific scenarios.

![NYC_ROAD_ACCIDENT_DASHBOARD]("")

---

## Key Metrics
1. **Total Reported Collisions**: 91,286
2. **Total Injuries**: 45,317
   - Persons Injured: 37,198
   - Pedestrians Injured: 4,211
   - Cyclists Injured: 1,932
   - Motorists Injured: 1,976
3. **Total Fatalities**: 276
   - Persons Killed: 213
   - Pedestrians Killed: 39
   - Cyclists Killed: 12
   - Motorists Killed: 12
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
