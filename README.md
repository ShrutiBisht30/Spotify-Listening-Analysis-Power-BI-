# Spotify Listening Analysis (Power BI)

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

## 📊 Data Summary  

- **Dataset**: Spotify listening history (CSV export)  
- **Time Period**: Covers multiple years of listening activity (from earliest to latest timestamp in the data).  
- **Rows**: Each row represents a single **play event** (when a track was started).  
- **Columns**: 11 attributes capturing metadata about the play event, track, and context.  

### 🔑 Key Points  
- Includes **track, artist, and album metadata**.  
- Captures **playback behavior** such as:  
  - Duration listened (`ms_played`)  
  - Start & end reasons (`reason_start`, `reason_end`)  
  - Engagement flags (`skipped`, `shuffle`)
### 📑 Data Dictionary 

| Column Name        | Description                                                | Datatype | Example Value                               |
|--------------------|------------------------------------------------------------|----------|---------------------------------------------|
| spotify_track_uri  | Unique identifier for track in Spotify (URI format).       | object   | 2J3n32GeLmMjwuAzyhcSNe                      |
| ts                 | Timestamp of when the track started playing.               | object   | 2013-07-08 02:44:34                         |
| platform           | Platform used to listen (e.g., web player, mobile, etc.).  | object   | web player                                  |
| ms_played          | Duration track was played in milliseconds.                 | int64    | 3185                                        |
| track_name         | Name of the track played.                                  | object   | Say It, Just Say It                         |
| artist_name        | Name of the artist of the track.                           | object   | The Mowgli's                                |
| album_name         | Name of the album containing the track.                    | object   | Waiting For The Dawn                        |
| reason_start       | Reason why playback started (autoplay, clickrow, nextbtn). | object   | autoplay                                    |
| reason_end         | Reason why playback ended (trackdone, unknown, nextbtn).   | object   | clickrow                                    |
| shuffle            | Whether shuffle mode was enabled (True/False).             | bool     | False                                       |
| skipped            | Whether the track was skipped (True/False).                | bool     | False                                       |


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

**Overview Dashboard**
[Overview](https://github.com/ShrutiBisht30/Spotify-Listening-Analysis-Power-BI-/blob/main/images/Overview.JPG?raw=true)
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
