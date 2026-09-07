# Medicare Part D Drug Spending Analysis: 2020–2024

## Project Overview

This project analyzes Medicare Part D prescription-drug spending from 2020 through 2024. The dashboard examines spending trends, prescription-claim volume, manufacturers, high-spending drugs, and changes in average spending per dosage unit.

The objective was to identify the drugs and manufacturers driving Medicare Part D spending and highlight drug products that may warrant additional cost review.

## Dashboard

<img width="1573" height="881" alt="image" src="https://github.com/user-attachments/assets/26afdbd1-49c8-43eb-b7c0-9681a43b9c2f" />

## Data Preparation

The original dataset stored separate spending and utilization columns for each year. Power Query was used to:

- Reshape the dataset from wide to long format
- Create a separate Year column
- Organize yearly measurements into consistent fields
- Rename columns and assign appropriate data types
- Distinguish overall drug totals from manufacturer-level records
- Prevent double-counting caused by the dataset's Overall summary rows

DAX was used to calculate weighted average spending per claim, distinct drug products, and growth in average spending per dosage unit.

## Dashboard Visualizations

- Total Spending, Total Claims, Average Spend per Claim, and Drug Products Analyzed
- Annual Medicare Part D Spending Trend
- Top 15 Drugs by Total Spending
- Top 10 Manufacturers by Total Spending
- Claims versus Average Spending per Claim scatterplot
- Top 10 Drugs by Growth in Average Spending per Unit
- Detailed drug and manufacturer table
- Filters for year, manufacturer, brand, generic name, and outlier status

## Questions Explored

- Which drugs account for the highest total spending?
- Which manufacturers account for the most spending?
- Is high spending associated with claim volume or high spending per claim?
- How did total spending change between 2020 and 2024?
- Which drugs experienced the greatest growth in average spending per dosage unit?
- Which drug products may warrant additional cost review?

## Data Source

The data was obtained from the Centers for Medicare & Medicaid Services:

- [Medicare Part D Spending by Drug](https://data.cms.gov/summary-statistics-on-use-and-payments/medicare-medicaid-spending-by-drug/medicare-part-d-spending-by-drug)
- [CMS Data Dictionary](https://data.cms.gov/resources/medicare-part-d-spending-by-drug-data-dictionary)
- [CMS Methodology](https://data.cms.gov/sites/default/files/2026-06/d7e0a571-9d08-40ec-8278-1b2300f59424/DSD_PTD_RY26_20260603_Methodology_WDDSE_508.pdf)
