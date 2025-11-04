# Marketing-Campaign-Analysis-Power-BI-Dashboard
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/f301988a-144f-49c7-aa61-67d8945329df" />

## 🔹 Project Overview  
This mini project analyzes how different **marketing campaigns** performed across regions and platforms (digital ads, social media, and traditional marketing).  
The goal is to evaluate **ROI, revenue, and spending** to identify the **best performing campaigns** and optimize marketing decisions.  

This project demonstrates skills in:  
- ✅ Data Cleaning & Transformation (Power Query)  
- ✅ Data Modeling (relationships across multiple tables)  
- ✅ DAX (custom measures for KPIs & ROI)  
- ✅ Dashboard Design (professional Power BI visuals, interactivity)  

---

## 📂 Dataset  
The project uses three CSV files:  
1. `Marketing_Campaign_Details.csv` – campaign information (type, duration, channel, etc.)  
2. `Marketing_Campaign_Performance.csv` – performance metrics (impressions, clicks, conversions, revenue, spend)  
3. `Region_Performance.csv` – region-wise attributes  

---

## 🛠 Data Preparation  
- Imported all CSV files into Power BI.  
- Cleaned data: renamed columns, corrected data types, handled nulls & duplicates.  
- Standardized column names (`CampaignName`, `CampaignType`, `Spend`, `Revenue`, etc.).  

---

## 🔗 Data Modeling  
Relationships built in the model:  
- `Marketing_Campaign_Details[CampaignName]` → `Marketing_Campaign_Performance[CampaignName]` (1:*).  
- `Region_Performance[Region]` → `Marketing_Campaign_Performance[Region]` (1:*).  

---

## 📐 DAX Measures  
Key measures created:  
- `Total Impressions`  
- `Total Clicks`  
- `Total Conversions`  
- `Total Revenue`  
- `Total Spend`  
- `Total ROI = (Revenue – Spend) / Spend`  
- `Average ROI`  
- `Best Campaign` (returns top campaign name by ROI)  

Additional optional metrics:  
- CTR = Clicks / Impressions  
- CPC = Spend / Clicks  
- CPA = Spend / Conversions  

---

## 📊 Dashboard Features  
The Power BI dashboard includes:  

- **Stacked Column Chart** – Spend vs Revenue by Region  
- **Combo Chart** – Spend & Avg ROI by Campaign  
- **Bar Chart** – ROI by Campaign  
- **Pie/Donut Chart** – Campaigns by Campaign Type  
- **Gauge Chart** – ROI vs Avg ROI  
- **KPI Cards** – Total Revenue, Total Spend, Average ROI, Best Campaign  
- **Slicers** – Filter by Region & Campaign Type  

🎨 **Design**:  
- Dark theme background with light text  
- Consistent formatting & styling (Format Painter)  
- Borders & shadows for distinction  


 

---

## 🔍 Key Insights  
- Campaign **X** delivered the highest ROI.  
- Region **Y** had high spend but low conversions.  
- Digital ads showed better ROI compared to traditional channels.  
- Recommendation: Reallocate budget towards high-performing campaigns while optimizing low ROI regions.  

---

