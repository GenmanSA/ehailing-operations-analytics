# ehailing-operations-analytics
An end-to-end data analysis project featuring data cleaning in Pandas, exploratory queries in SQL, and final business insights in power bi.

# 🚖 Pretoria E-Hailing Operations Analytics (1M Trip Simulation)

**A comprehensive data analytics pipeline simulating 1 million e-hailing trips over 365 days to model driver behavior, geographic safety risks, and platform unit economics in Gauteng, South Africa.**

## 📌 The Business Problem
E-hailing platforms in South Africa face unique operational challenges that impact driver retention, passenger safety, and platform profitability. Drawing on domain expertise from the Pretoria market, this project analyzes 1 million simulated trip records across 1,000 drivers to solve core friction points:
*   **Safety & Geo-Conflict:** Taxi violence at major transit hubs (e.g., Bosman Station).
*   **Unit Economics:** The profitability trap of long-haul airport trips vs. public transit (Gautrain).
*   **Supply vs. Demand:** Flaws in micro-burst bonuses, temporal hyper-demand (weekend nightlife), and passenger wait-time tolerance.

## 🛠️ Tech Stack & Methodology
*   **Python (Pandas, Numpy):** Programmatically generated 1 million realistic trip records. Engineered features including dynamic pricing, wait times, and maintenance habits.
*   **Data Cleaning:** Built a preprocessing pipeline to handle missing categorical data, standardize datetimes, and filter GPS outliers.
*   **SQL (SQLite / CTEs):** Executed 9 advanced queries to compress 1 million rows into lightweight summary tables, optimizing performance for BI rendering.
*   **Power BI:** Designed a 3-tab interactive dashboard tracking Safety, Platform Economics, and Operational Efficiency.

## 📊 Key Strategic Insights

1. **Dynamic Geo-Fencing (Bosman Station):** Data proves a massive revenue bleed in High-Risk Zones due to driver cancellations. *Recommendation:* Implement a 200m geo-fence around Bosman directing passengers to safe pick-up nodes.
2. **Macro-Volume Targets vs. Micro-Burst Bonuses:** Replacing flawed 2-hour burst bonuses with a R1,000 macro-volume target (e.g., 500 trips) stabilizes 24/7 supply and eliminates peak-hour cherry-picking.
3. **The OR Tambo Profitability Trap:** Long-haul airport trips operate at a net loss for drivers after 28.5% platform fees and R5/km petrol costs. *Recommendation:* Introduce an Intercity Base Fare (R450) to remain competitive with Gautrain while restoring driver profit margins.
4. **Friday Night Hyper-Demand:** Heatmap analysis shows massive revenue bleed on Friday/Saturday nights. This isn't due to city-wide danger, but a severely stretched supply. Geo-fencing Bosman frees up drivers to service the highly profitable, safe nightlife routes.

## 📂 Repository Structure

```text
ehailing-operations-analytics/
│
├── data/
│   ├── ehailing_1M_trips_data.csv.zip  # Raw data (1M rows, 365 days)
│   └── ehailing_1M_cleaned.csv.zip     # Cleaned data
│
├── scripts/
│   ├── 01_data_generator_1M.py         # Python simulation script 
│   └── 02_data_cleaning.py             # Preprocessing pipeline
│
├── sql/
│   ├── 1_risk_zones.sql                
│   ├── 2_car_wash_roi.sql              
│   ├── 3_volume_bonus.sql              
│   ├── 4_wait_time_tolerance.sql       
│   ├── 5_surge_elasticity.sql          
│   ├── 6_vehicle_tiers.sql             
│   ├── 7_time_of_day.sql               
│   ├── 8_peak_time_revenue_bleed.sql   # Heatmap query
│   └── 9_unit_economics.sql            # OR Tambo vs Gautrain query
│
├── visuals/
│   └── PowerBI_Dashboard_Screenshots/
│
└── E-Hailing_Insights_Memo.pdf         # Executive summary
