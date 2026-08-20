# Public Transport Delay Analysis Dashboard 🚌🚆
### Built entirely in Microsoft Excel

## 📌 Project Overview
This project analyzes **~2,000 public transport trip records** (buses, trams, metros, and trains) to understand what drives arrival and departure delays. The entire analysis — from raw data cleaning to pivot tables, charts, and a final interactive dashboard — was built **100% in Excel**, using PivotTables, PivotCharts, and slicers for interactivity.

## 🎯 Key Objectives
- Identify which factors are most associated with transport delays — transport type, weather, weekday, season, peak hour, and traffic congestion.
- Compare on-time performance across different routes and transport modes.
- Build a single-page interactive dashboard to explore delay patterns visually.

## 🛠️ Technologies Used
| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Data cleaning, PivotTables, PivotCharts, and dashboard design |
| **PivotTables & PivotCharts** | Aggregating delays by category |
| **Slicers** | Interactive filtering on the dashboard |

## 📁 Dataset
The raw dataset (`RawData` sheet) contains trip-level records with fields including:
- Trip ID, date, time, transport type, route, origin/destination stations
- Scheduled vs. actual departure/arrival delay (minutes)
- Weather condition, temperature, humidity, wind speed, precipitation
- Event type & estimated attendance nearby
- Traffic congestion index, holiday/peak-hour/weekday flags, season
- Delay flag and congestion level (Low/Medium/High)

## 📊 Analysis Breakdown
The workbook includes dedicated pivot sheets analyzing delay by:
- **Transport type** (arrival & departure)
- **Weather condition** (arrival & departure)
- **Peak hour** (arrival & departure)
- **Congestion level**
- **Weekday**
- **Season**
- **Event type**
- **Holiday**
- **Route performance** — top/bottom performing routes
- **Top 5 delayed routes**

## 📈 Dashboard
A consolidated **Dashboard** sheet brings all of the above together into a single interactive view with charts and slicers, so you can filter delay trends by transport type, weather, season, and more without touching the underlying pivot tables.

## 📁 Repository Structure
```
├── Public-Transport-Delay-Analysis/
│   ├── Public_Transport_Delay_Dashboard.xlsx
│   ├── RawData.xlsx
│   ├── Congestion-Arrival.xlsx
│   ├── EventType_Arrival.xlsx
│   ├── Holiday_Arrival.xlsx
│   ├── PeakHour_Arrival.xlsx
│   ├── PeakHour_Departure.xlsx
│   ├── Season_Arrival.xlsx
│   ├── Top5Routes.xlsx
│   ├── TransportType_Arrival.xlsx
│   ├── TranportType_Departure.xlsx
│   ├── Weather_Arrival.xlsx
│   └── Weather_Departure.xlsx
└── README.md
```

## 🚀 How to Use
1. Download `Public_Transport_Delay_Dashboard.xlsx` and open it in Microsoft Excel (slicers and PivotCharts work best in Excel, not Google Sheets).
2. Go to the **Dashboard** sheet.
3. Use the slicers to filter by transport type, weather, weekday, season, or peak hour and explore how delays shift.
4. Individual pivot sheets (e.g., `Weather_Arrival`, `RoutePerformance`) can be explored for a deeper breakdown of any one factor.

---
*Feel free to connect if you have suggestions or feedback on this project!*
