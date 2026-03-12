# Australian Energy Market Analysis (Victoria 2025)

## Overview
This project analyses Victorian electricity market data using SQL and Python. 
Real data from AEMO (Australian Energy Market Operator) was loaded into a 
SQLite database and queried to uncover demand and pricing trends across 2025.

## Dataset
- **Source:** AEMO Price and Demand Data
- **Region:** Victoria (VIC1)
- **Size:** 105,120 rows of 5-minute interval data across 12 months

## Key Questions
- How does electricity demand and price vary across months?
- What time of day sees the highest energy demand?
- Which days had the most extreme price spikes?
- Does high demand always lead to high prices?

## Key Findings
- **Winter months (June, July) have the highest demand** — peaking at 5941 MW average in July
- **June had an extreme price spike** — average of $264/MWh vs $27/MWh in December
- **6pm is the peak demand hour** across the year — the classic evening peak
- **Prices only spike at extreme demand levels** (above ~7000 MW) — below that the market stays stable

## Visualisations

### Monthly Energy Demand and Price
![Monthly Demand and Price](Visuals/Monthy%20energy%20demand%20%26%20price.png)

### Demand by Hour
![Demand by Hour](Visuals/Demand%20by%20hour.png)

### Energy Demand vs Price
![Energy Demand vs Price](Visuals/Energy%20demand%20by%20price.png)


## Tools Used
- Python (Google Colab)
- SQL (SQLite)
- Pandas
- Matplotlib

## How to Run
1. Download Victoria 2025 data from [AEMO](https://aemo.com.au)
2. Upload all 12 CSV files to Google Colab
3. Run all cells in `energy_market_analysis.ipynb`
