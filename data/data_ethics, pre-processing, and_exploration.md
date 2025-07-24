# 🚗 NYC Motor Vehicle Collisions Analysis

A comprehensive data analysis and visualization project exploring motor vehicle collisions in New York City. This project highlights data cleaning, visualization, and geospatial mapping techniques, with attention to data ethics and responsible usage.

---

## 📊 Objectives

- Identify top contributing crash factors
- Detect patterns across boroughs and vehicle types
- Analyze temporal trends (hour/day/month)
- Map geographic crash hotspots
- Visualize crash severity (injuries and fatalities)

---

## 📁 Dataset

**Source:** NYC Open Data  
**File:** `Motor_Vehicle_Collisions_-_Crashes_20241229.csv`

---

## 🧹 Step 1: Data Preparation & Preprocessing

- Convert date/time fields to datetime format
- Remove rows with missing geographic coordinates (for mapping)
- Handle and quantify missing values
- Generate summaries and extract relevant features like:
  - Hour of Day
  - Day of Week
  - Crash Type (Injury, Fatality)

---

## 🔐 Step 2: Data Ethics

- ⚠️ This dataset contains **sensitive public safety information**
- No personal data is used
- Always aggregate before visualization
- Location-based visualizations are presented at a **city-wide level** only
- This project is for **educational and public safety analysis purposes only**

---

## 📈 Step 3: Exploratory Data Analysis

- 🚘 Top contributing crash factors
- 🚐 Vehicle types most involved
- 🕓 Crashes by time of day/week
- 🗺️ Heatmaps by crash location and severity
- 📅 Trend decomposition over time

---

## 🌐 Interactive Visualizations

- **Heatmap of Crash Locations:** `visualizations/Heatmap.html`
- **Crash Severity Map:** `visualizations/severity.html`

---

## ⚙️ Requirements

```bash
pandas
matplotlib
seaborn
folium
statsmodels
