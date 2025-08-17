# 🎵 Spotify Listening Analysis (Power BI)

## 📌 Objectives
- Transform raw Spotify listening history into **actionable insights**.  
- Identify listening patterns across **albums, artists, and tracks**.  
- Analyze **engagement trends** (weekend vs weekday, skipped vs not, shuffle vs not).  
- Build a **scalable Power BI model** using dynamic date tables & advanced DAX.  

---

## 🛠️ Tools Used
- **Power BI** → Data modeling, visualization, DAX  
- **Power Query** → Data cleaning & transformation  
- **DAX** → Measures, KPIs, conditional formatting  
- **CSV Dataset** → Spotify streaming history  

---

## 🔄 Process
1. **Data Cleaning & Modeling**
   - Imported CSV, checked datatypes, removed unnecessary columns.  
   - Split timestamp → `Track Played Date` & `Track Played Time`.  
   - Created **dynamic Date Table** with CALENDAR().  

2. **Feature Engineering**
   - Extracted **Year, Day Name, Weekday/Weekend, Hour**.  
   - Built relationships for **time intelligence functions**.  

3. **DAX Measures**
   - Distinct counts for Albums, Artists, Tracks.  
   - YoY growth KPIs.  
   - Dynamic Min/Max labels in trend charts.  
   - Quadrant segmentation for **high engagement tracks**.  

4. **Report Pages**
   - **Overview** → Albums, Artists, Tracks (KPIs, trends, favorites).  
   - **Listening Patterns** → Heatmap (Day vs Hour), Scatter (Avg time vs Frequency).  
   - **Drill-through** → Detailed breakdown by Album, Artist, Track, Platform, Date.    

---

## 🖼️ Screenshots  

- Overview Dashboard  
- Listening Patterns Heatmap  
- High Engagement Tracks Scatter Plot  

---

## 🚀 Outcomes
- Delivered a **business-ready, Spotify-themed Power BI dashboard**.  
- Showcased **data storytelling** through design & branding.  
- Demonstrated ability to handle **end-to-end BI workflow**: cleaning → modeling → insights.  

---

👩‍💻 **Author**: Shruti Bisht  
📊 *Data Analyst*  
