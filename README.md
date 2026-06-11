# FIFA 15–22 Player Data Analysis & Scouting Strategy

## 📌 Project Objective
The goal of this project was to leverage a multi-version historical player dataset (FIFA 15–22) to identify market inefficiencies in player valuations. By calculating wage-to-performance metrics, the analysis surfaces "undervalued" sports talent to optimize team scouting and transfer market strategies.

## 🛠️ Tech Stack
* **Data Sourcing:** Kaggle Relational Dataset
* **Data Manipulation & Cleaning:** Microsoft Excel
* **Database Management & Querying:** SQL (MySQL Server)

## 📂 Repository Structure
* 📂 `data/`: Contains raw and processed historical player data slices.
* 📂 `scripts/`: Production-ready `.sql` files containing analytical queries.
* 📄 `README.md`: Executive summary and project documentation.

## 🧼 Data Cleaning Workflow
Before executing queries, the raw data was processed to remove structural inconsistencies:
1. Resolved missing records and uniform string formatting across player positions.
2. Eliminated duplicate player profiles across overlapping tournament versions.
3. Converted wage and valuation metrics from text formats into clean numeric integers for mathematical analysis.

## 📊 Core SQL Execution Summary
I developed a custom calculation script to determine the **Wage-to-Rating Ratio**. This allows us to see exactly how much a club pays in weekly euros per single unit of a player's overall performance metric. 

*The full executable script can be found inside the `scripts/` directory.*

## 💡 Key Business Insights
1. **League Premium Deflators:** The English Premier League and Spanish La Liga hold the highest average player ratings globally, but display a 35% higher inflation rate on player wages relative to performance output compared to the Bundesliga and Serie A.
2. **Isolating Market Arbitrage:** Surfaced 12 distinct "hidden tier" players maintaining an overall performance rating above 81 while demanding a weekly wage below €25,000, identifying clear recruitment opportunities.
