# SmartSupply — Supply Chain Network Analysis and Decision Support

## Project Overview

SmartSupply is a supply chain analytics project developed using Microsoft Excel and Power BI. It examines order quantities, plant-level demand, daily plant capacity, warehouse cost per unit, plant-port relationships, and product sourcing flexibility.

The goal is to organize supply chain data into an analytical workbook and an interactive dashboard to support exploration and decision-making.

## Tools Used

- Microsoft Excel — data analysis, summaries, and pivot tables
- Microsoft Power BI Desktop — dashboard visualizations and plant selection
- Power Query — data preparation and transformation

## Dataset

The project uses a supply chain logistics dataset attributed to Brunel University London. The workbook contains tables covering orders, freight rates, warehouse costs, warehouse capacities, products per plant, vendor-managed-inventory customers, and plant-port relationships.

## Analysis Performed

- Analysed 9,215 order records.
- Summarized approximately 29.51 million units of recorded order quantity.
- Identified 772 unique products.
- Examined demand distribution across the seven plants included in the plant-demand summary.
- Reviewed daily capacity information for 19 plants.
- Compared warehouse cost-per-unit values across the plant network.
- Examined relationships between plants and ports.
- Summarized product sourcing flexibility by the number of supplying plants.

## Key Findings

- The dataset contains 9,215 orders and approximately 29.51 million units of recorded order quantity.
- The plant-demand summary attributes approximately 96.9% of recorded order quantity to PLANT03.
- The sourcing-flexibility summary contains 772 products: 503 associated with one supplying plant, 141 with two, 43 with three, 71 with four, and 14 with five.
- Therefore, 503 of 772 products (approximately 65.2%) fall into the one-supplying-plant category in this summary.
- Warehouse cost per unit varies across the 19 plants represented in the warehouse-cost data.

## Power BI Dashboard

The report includes:

- KPI cards for total orders, total quantity, unique products, and number of plants in the network
- A plant selector listing 19 plant codes
- Bar charts for order quantity by plant, daily capacity by plant, and warehouse cost per unit by plant
- A pie chart showing order quantity share by plant
- A donut chart summarizing product sourcing flexibility
- A key insights section

The dashboard uses a dark theme with contrasting chart colours.

## Limitations

- The plant-demand summary currently contains seven plants, while the plant selector and capacity/cost data cover 19 plants. The demand pie chart therefore represents the plants included in that summary, not all 19 plants.
- The warehouse-cost chart does not currently respond to the shared plant selector.
- The sourcing-flexibility donut is an overall summary and is not broken down by individual plant.
- The order records share the same recorded date, so the analysis should not be interpreted as a time-series trend.
- Order quantities and daily capacity use different measures and should not be compared directly without appropriate time and unit alignment.
- This project presents descriptive analysis and dashboard-based decision support. It does not claim to have implemented an optimization algorithm or measured cost savings or emissions reductions.

## Project Files

- `SmartSupply_Dashboard.pbix` — Power BI report
- `SmartSupply_Analysis.xlsx` — Excel analysis workbook

## Future Improvements

Potential next steps include refining the Power BI data model so the plant selector filters compatible visuals consistently, validating freight-rate matching, and developing a documented optimization approach if suitable assumptions and constraints are established.
