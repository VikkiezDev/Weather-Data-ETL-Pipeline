# Weather-Data-ETL-Pipeline ![Project Status](https://img.shields.io/badge/status-WIP-yellow.svg)

A comprehensive Power BI dashboard that analyzes over a decade of Indian weather data across various regions and seasons. The project highlights climate variability, seasonal patterns, and long-term meteorological shifts to support data-driven decision-making in agriculture, infrastructure, energy, and policy planning.

---

## 📁 Project Structure
├── data/
│ └── output_data.csv # Final cleaned and transformed weather dataset
├── dashboard/
│ └── India_Weather.pbix # Power BI dashboard file
├── scripts/
│ └── extract.py # Python-based ETL (data cleaning, reshaping)
│ └── transform.py # Python-based ETL (data cleaning, reshaping)
│ └── load.py # Python-based ETL (data cleaning, reshaping)
├── config/
│ └── config.py # Chart descriptions and analytical insights
├── main.py
└── README.md


---

## 🧠 Key Objectives

- Visualize seasonal and annual weather fluctuations across regions.
- Detect anomalies (e.g., unseasonal rainfall, heatwaves, cold spells).
- Analyze climate trends for agriculture, infrastructure, and energy planning.
- Identify correlations between weather parameters (e.g., rainfall vs temperature).

---

## 🛠️ Tools & Technologies

- **Python (Pandas)** – Data transformation, formatting, and preprocessing
- **Google Cloud Storage** - Storage cloud bucket
- **Snowflake (Optional)** – Scalable cloud-based data warehousing
- **Cron** - Automation
- **Power BI** – Business intelligence and interactive visualizations
- **Git/GitHub** – Version control and project collaboration
- **CSV File** – Cleaned structured weather data

---

## 📈 Core Visualizations

| Chart Type              | Purpose                                                             |
|-------------------------|---------------------------------------------------------------------|
| Line Chart              | Temperature, humidity, and rainfall trends over time                |
| Area Chart              | Seasonal patterns and climatic cycles                               |
| Heatmap Matrix          | Intensity mapping of rainfall/temperature by month & year           |
| Bar Chart               | Region-wise distribution of climatic variables                      |
| Slicer Panel            | Dynamic filtering by state, year, season                           |
| KPI Cards               | Max/Min Avg Temp, Cumulative Rainfall, Annual Extremes              |
| Decomposition Tree      | Drill-down analysis by State → District → Season                   |
| Waterfall Chart         | Year-over-year change in rainfall/temperature                       |
| Correlation Plot        | Weather parameter inter-dependencies                                |

---

## 🌐 Dataset Summary

- **Time Frame**: 2011–2023 (Monthly/Quarterly)
- **Columns**: `Item`, `Value`, `Year`, `Quarter`, `Metric`, `Date`
- **Measured Parameters**:
  - Rainfall (mm)
  - Temperature (°C)
  - Humidity (%)
  - Wind Speed (km/h)
  - Pressure (hPa)
- **Geographies**:
  - Pan-India coverage (State-wise or District-wise depending on granularity)

---

## 🔍 Insights & Observations

- ☔ 2020–21 saw record rainfall deviations in monsoon season (La Niña effect)
- 🔥 Noticeable rise in average summer temperatures post-2016 in northern states
- 🌾 Rainfall pattern shifts have direct implications for sowing cycles
- 🌬️ Wind speed variations higher in coastal belts during Q2 and Q3
- ❄️ Cooler winters becoming shorter — possible sign of climate compression

---

## 🚀 How to Run Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/india-weather-powerbi.git
   cd india-weather-powerbi
   ```
