🚖 South African E-Hailing Operations, Safety & Driver Economics (2016 vs. 2026)
An end-to-end Data Analytics & Unit Economics portfolio project analyzing 2,000,000 simulated e-hailing trips across Gauteng (Pretoria & Johannesburg) to quantify 10-year driver margin compression, taxi rank conflict zones, telematics ROI, and temporal revenue cyclicity.

📌 Executive Summary & Business Problem
Between 2016 and 2026, the South African e-hailing industry experienced a severe economic decoupling. While per-kilometer passenger fares dropped due to aggressive price wars (Uber Go / Bolt Economy rates averaging ~R4.60–R5.40/km vs. R7.80/km in 2016), operating costs surged:

Fuel Inflation: Petrol increased +128% (from R12.50/L in 2016 to R28.50/L in 2026).
Platform Take-Rate: Effective deductions (commission + booking/service levies) climbed from 20% to ~38%.
The Weekly Vehicle Lease Trap: 78% of drivers lease their cars, paying vehicle owners R1,500–R2,200/week for budget hatchbacks (Suzuki Swift, Toyota Vitz), R2,500–R3,500/week for sedans (Toyota Corolla Quest, Nissan Almera), and R6,000–R8,500+/week for Uber Black & Luxury Vans.
Violent Taxi Rank Friction: Pickups at Bosman Gautrain/Taxi Rank (Pretoria CBD), Park Station / Noord Rank (Joburg CBD), Mamelodi, and Germiston suffer ~75% cancellation rates due to violent intimidation and chases by roaming taxi patrol squads.
🛠️ Tech Stack & Analytics Architecture
Python (Pandas, NumPy): Vectorized, memory-optimized synthetic data engineering modeling Gauteng spatial corridors, payday cycles, stadium events, and vehicle telematics.
SQL (DuckDB): High-speed in-memory SQL aggregations evaluating unit economics, cancellation bleed, and fleet lease deductions.
Data Visualization (Matplotlib, Seaborn): 8 side-by-side Problem vs. Solution executive dashboard pairs.
📊 Key Analytical Findings & Strategic Solutions
1. Gauteng Taxi Rank Conflict Zones vs. 250m Dynamic Geofencing
Taxi Ranks & Geofencing

The Problem: Bosman Station (Pretoria), Park Station (Joburg), Mamelodi, and Pretoria West/North experience ~75% cancellation rates, while Sunnyside/CBD experiences high request volumes but heavy taxi friction. Conversely, Centurion Gautrain, Sandton Gautrain, Brooklyn, Pretoria East, and Rosebank operate safely with <18% cancellations.
The Solution: Deploy a 250m Dynamic Geofence around high-risk taxi ranks and Bosman Station, routing riders to designated, camera-monitored Safe Pick-Up Nodes.
2. Monthly Revenue Cyclicity: The 25th–5th Payday Boom vs. 6th–24th Slump & Stadium Spikes
Payday & Stadium Spikes

The Problem: Platform revenue collapses between the 6th and 24th of every month, whereas drivers generate 2.4x–3.0x higher daily revenue between the 25th and 5th (salary window).
The Solution: Counteract the mid-month slump by deploying targeted event surge zones around weekend rugby and soccer blockbusters (Loftus Versfeld Vodacom Bulls/Sundowns matches and FNB Stadium / Ellis Park Soweto Derbies & Springbok Tests).
3. 10-Year Driver Exploitation (2016 vs. 2026) & Weekly Owner Lease Deductions
Driver Exploitation & Leases

The Problem: Net profit per 10km standard trip collapsed by -63.3% (from R68.40 in 2016 to R25.10 in 2026) before deducting the R1,500–R8,500 weekly owner lease.
The Solution: Index base per-km fares to inland petrol price adjustments and cap effective platform take-rates at 25% for drivers meeting monthly safety and volume tiers.
4. Panic Buttons vs. Police Visibility & South African Tracker Recovery Rates
Panic Buttons & Trackers

The Problem: Static police visibility near stations reduces taxi chase danger by <2% because roaming rank squads follow e-hailing cars away from precincts. Untracked vehicles suffer an 82% total loss rate in hijackings/severe crashes.
The Solution: Partner with top South African telematics providers (Cartrack R199/pm, Netstar R169/pm, Tracker SA R249/pm, Matrix R219/pm), boosting vehicle recovery to 92%+ and raising driver threat escape rates from 34% to 89% via in-vehicle armed-response Panic Buttons.
5. The OR Tambo Airport Long-Haul Trap vs. Gautrain Pricing
OR Tambo Unit Economics

The Problem: Long-haul trips (45km+) from Pretoria to OR Tambo International Airport force drivers to absorb empty return ("deadhead") fuel costs at R28.50/L.
The Solution: Introduce a R450 Intercity Flat Base Fare, restoring driver net margins while remaining 17% cheaper for two passengers than two Gautrain tickets (~R540 total).
6. Vehicle Cleanliness ROI & 500-Trip Macro Bonus Gamification
Cleanliness & Bonus Gamification

The Problem: Unwashed cars suffer a 3.95★ average rating (risking platform deactivation below 4.2★), while 2-hour morning micro-bonuses cause mid-day supply deserts.
The Solution: Replace micro-burst bonuses with a 500-Trip Monthly Macro Bonus (R1,000 fuel credit + subsidized car wash vouchers), lifting ratings to 4.78★ and cutting cancellations by 9%.
7. Weekend Nightlife Revenue Bleed Heatmap & Passenger Wait-Time Cliff
Heatmap & Wait Tolerance

The Finding: Passengers cancel exponentially once wait times exceed 9 minutes, causing severe weekend nightlife revenue bleed in Brooklyn, Hatfield, Rosebank, and Sandton.
8. Fleet Composition & Corridor Passenger Demographics
Fleet & Demographics

The Finding: Suzuki Swift (28%) and Toyota Vitz (22%) dominate the Gauteng Economy fleet, while Toyota Corolla Quest (16%) leads Standard UberX/Bolt operations.
