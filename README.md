# Public Transport Delay Analysis Dashboard 🚌🚆
### Built entirely in Microsoft Excel

## 📌 Project Overview
This project analyzes **~2,000 public transport trip records** (buses, trams, metros, and trains) to understand what drives arrival and departure delays. The entire analysis — from raw data cleaning to pivot tables, charts, and a final dashboard — was built **100% in Excel**, using PivotTables, PivotCharts, and interactive slicers within individual analysis sheets.

## 🎯 Key Objectives
- Identify which factors are most associated with transport delays — transport type, weather, weekday, season, peak hour, and traffic congestion.
- Compare on-time performance across different routes and transport modes.
- Build a single-page dashboard to explore delay patterns visually.

## 🛠️ Technologies Used
| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Data cleaning, PivotTables, PivotCharts, and dashboard design |
| **PivotTables & PivotCharts** | Aggregating delays by category |
| **Slicers** | Interactive filtering within individual pivot analysis sheets |

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
- **Top 5 delayed routes**

Public-Transport-Delay-Analysis/
│
├── Public-Transport-Delay-Analysis/
│ ├── Public_Transport_Delay_Dashboard.xlsx
│ ├── RawData.xlsx
│ ├── Congestion-Arrival.xlsx
│ ├── EventType_Arrival.xlsx
│ ├── Holiday_Arrival.xlsx
│ ├── PeakHour_Arrival.xlsx
│ ├── PeakHour_Departure.xlsx
│ ├── Season_Arrival.xlsx
│ ├── Top5Routes.xlsx
│ ├── TransportType_Arrival.xlsx
│ ├── TranportType_Departure.xlsx
│ ├── Weather_Arrival.xlsx
│ └── Weather_Departure.xlsx
│
├── Dashboard.png
└── README.md

## 📈 Dashboard
A consolidated **Dashboard** sheet brings all of the above together into a single overview view with KPI cards and charts, so you can see delay trends across transport type, weather, season, congestion, weekday, and top problem routes at a glance.

## 💡 Key Business Insights

- 📅 **Weekday is the strongest driver of delay found in this dataset.** Average arrival delay ranges from 12.31 min to 14.31 min across the week — a 2-minute (~15%) swing — making it the most actionable pattern identified. *(Note: the numeric weekday-to-day mapping wasn't confirmed in the source data, so specific days aren't named here.)*
- 🍂 **Season shows a moderate effect.** Autumn trips average 13.89 min delay vs. 12.72 min in Summer — worth monitoring but not a dominant factor.
- 🎪 **Event type shows a moderate, if noisy, pattern.** Protests and parades correlate with the highest delays (13.90 and 13.62 min), while concerts, sports, and festivals actually show *lower* delays than trips with no nearby event — possibly reflecting better transit planning around scheduled events, though this needs further investigation before drawing firm conclusions.
- 🚌 **Transport type, weather condition, and congestion level have minimal individual impact on delay** (spreads of 0.46–0.75 min, roughly 3–6% of the average). Notably, "High" congestion trips were *not* the most delayed — congestion index alone is a weak predictor here.
- ⏰ **Peak hour has essentially no effect on delay** (13.30 vs. 13.36 min) — a negligible 0.06-minute difference.
- 🛣️ **Route_12 is the single worst-performing route** at 14.29 min average delay, 2.48 minutes worse than the best route (Route_10 at 11.81 min) — a route-specific issue worth investigating independently of system-wide factors. *(Based on full route analysis conducted during the project; the Top 5 worst routes are available in `Top5Routes.xlsx`.)*
- ⚠️ **74.95% of all trips experienced some delay**, though the *magnitude* of delay is driven more by day-to-day and route-specific variation than by transport mode, weather, or congestion alone.

*Note: these insights are based on comparing average delays across categories, not formal statistical significance testing — so some smaller patterns (like Season or Event Type) should be treated as directional rather than confirmed.*

## 📝 Conclusion
Across ~2,000 trips, delays appear to be driven primarily by **when** (weekday, season) and **where** (specific routes) rather than **how** people travel or prevailing traffic/weather conditions. Transport type, weather, congestion, and peak hour each individually explain very little variation in delay — suggesting that isolated operational factors aren't the main lever for improvement. Instead, targeted investigation into high-delay weekdays and consistently underperforming routes like Route_12 would likely yield the most actionable improvements for transit reliability.

## 🚀 How to Use
1. Download `Public_Transport_Delay_Dashboard.xlsx` for an at-a-glance overview of KPIs and key charts.
2. Download any individual analysis file (e.g., `Weather_Arrival.xlsx`, `Congestion-Arrival.xlsx`, `Top5Routes.xlsx`) separately to explore that specific factor in more depth — each includes a working slicer to filter the data interactively.
3. All files are standalone and can be opened independently in Microsoft Excel.

---
*Feel free to connect if you have suggestions or feedback on this project!*

