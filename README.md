# Dubai Metro Ridership Recovery Analysis (2019 vs 2024)

## 📌 Project Overview
This project analyzes post-COVID ridership recovery across Dubai Metro stations using official RTA data. The goal was to identify which stations have fully recovered, which have surpassed pre-pandemic levels, and which are lagging behind.

## 🛠️ Tools Used
* **MySQL:** Data cleaning, deduplication, and aggregation.
* **Tableau Public:** Interactive dashboard creation and data visualization.

## 🔍 Key Insights
1. **Commuter Stations are Booming:** Stations in developing residential/commercial areas (e.g., Energy Metro Station at +168%, Al Jadaf at +115%) have significantly surpassed their 2019 baselines.
2. **Tourist Stations are Lagging:** Stations heavily dependent on tourism (e.g., Burj Khalifa/Dubai Mall at 74.9%, World Trade Centre at 71.7%) are still recovering toward pre-pandemic levels.
3. **System-Wide Recovery:** Overall system ridership has successfully rebounded and exceeded 2019 levels, showing the resilience of Dubai's public transport network.

## 🧹 Data Quality Challenges (The "Hidden" Work)
* The raw RTA dataset contained multiple duplicate snapshots per month (identified via `load_timestamp`). 
* I used SQL `MAX()` aggregations grouped by station/year/month to deduplicate the data before calculating the recovery baselines, ensuring accurate trend analysis.

## 🔗 Links
* [View the Interactive Tableau Dashboard Here](PASTE_YOUR_TABLEAU_PUBLIC_LINK_HERE)

## 📊 Dashboard Preview
![Dashboard](dashboard.png)
