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

## Key Findings

- The analysis covers 3,625 drug products, 7.81 billion claims, and approximately $1.21 trillion in total spending, with a weighted average of $155.26 per claim.
- Annual Medicare Part D spending increased from approximately $193 billion in 2020 to $289 billion in 2024—an increase of about 50%.
- Eliquis, an anticoagulant used to reduce the risk of strokes and blood clots, had the highest total spending at approximately $77 billion.
- Jardiance, used for type 2 diabetes and certain heart and kidney conditions, ranked second at $32 billion, followed by the type 2 diabetes medication Ozempic at $31 billion.
- BMS Primarycare led manufacturers with approximately $83 billion in spending, followed by Novo Nordisk ($74 billion) and Boehringer Ingelheim ($66 billion).
- High claim volume was generally associated with lower average spending per claim, while the highest-cost drugs tended to have substantially fewer claims.
- Lagevrio, an antiviral authorized for certain high-risk adults with mild-to-moderate COVID-19, had the greatest increase in average spending per dosage unit from 2023 to 2024.
- Jynneos, a vaccine for preventing smallpox and mpox, and Unasyn, an injectable antibiotic for bacterial infections, also showed substantial growth and may warrant further cost review.

## Data Source

The data was obtained from the Centers for Medicare & Medicaid Services:

- [Medicare Part D Spending by Drug](https://data.cms.gov/summary-statistics-on-use-and-payments/medicare-medicaid-spending-by-drug/medicare-part-d-spending-by-drug)
- [CMS Data Dictionary](https://data.cms.gov/resources/medicare-part-d-spending-by-drug-data-dictionary)
- [CMS Methodology](https://data.cms.gov/sites/default/files/2026-06/d7e0a571-9d08-40ec-8278-1b2300f59424/DSD_PTD_RY26_20260603_Methodology_WDDSE_508.pdf)
