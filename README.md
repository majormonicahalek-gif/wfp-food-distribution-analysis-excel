# WFP Food Distribution Analysis: Kakuma & Kalobeyei

An end-to-end Excel analysis of WFP food assistance across the Kakuma Refugee Camp and Kalobeyei Integrated Settlement in Turkana County, Kenya (January 2023 to December 2025). It includes a cleaned dataset, pivot table analysis, and an interactive Excel dashboard for WFP management.

![Dashboard preview]![Uploading image.png…<img width="840" height="457" alt="Screenshot 2026-11-10 104404" src="https://github.com/user-attachments/assets/7b9fe2c0-dba5-40f8-a030-98976c67a4e3" />
]


## Business Problem

The refugee population in Kakuma and Kalobeyei keeps changing through new arrivals, relocations, births, and departures. WFP management wants to know how food is distributed across locations and nationalities, how distribution has trended over time, and where operations can be improved.

## Business Questions

1. How many households received food assistance?
2. How many beneficiaries were reached?
3. Which locations received the most food?
4. Which nationalities received the most food assistance?
5. Which commodities were distributed most?
6. How has distribution changed over time?
7. Which distribution centers serve the most beneficiaries?
8. Are there locations experiencing delays?
9. What is the average quantity of food per household?
10. What would improve distribution operations?

## Dataset

| Item | Detail |
|---|---|
| Records | 15,000 household distribution records |
| Period | Jan 2023 to Dec 2025 |
| Locations | Kakuma 1 to 4, Kalobeyei Village 1 to 3 |
| Fields | Distribution_ID, Date, Location, Distribution_Center, Nationality, Household_Head_Gender, Household_Size, Beneficiaries, Food_Commodity, Quantity_KG, Distribution_Status, Delay_Days |

## Approach

1. **Data cleaning:** checked for duplicates, missing values, inconsistent nationality names, date formats, unusual food quantities, and location categories.
2. **Calculations:** built in a Working Sheet using `SUMIF`, `COUNTA`, `TEXT` (month), and `YEAR` (year).
3. **Pivot tables:** 12 PivotTables in a Summary sheet for location, nationality, month, commodity, distribution center, household head gender, and status.
4. **Dashboard:** KPI cards linked to the pivots with `GETPIVOTDATA`, 8 charts, and interactive slicers for Year, Month, Location, Nationality, Food Commodity, and Distribution Center.

## Key Metrics

| Metric | Value |
|---|---|
| Households served | 15,000 |
| Beneficiaries reached | 165,043 |
| Total food distributed | 3,865,388 kg |
| Average food per household | 257.7 kg |
| Distribution centers | 10 |
| Completion rate | 33.9% |
| Average delay (delayed records) | 7.0 days |

## Dashboard Visuals

- Interactive slicers (Year, Month, Location, Nationality, Food Commodity, Distribution Center)
- Food Distribution by Location
- Beneficiaries by Nationality
- Monthly Food Distribution Trend
- Food Distribution by Commodity
- Households Served by Location
- Distribution by Household Head Gender
- Distribution Centers by Beneficiaries
- Average Food Distributed by Location

## Key Findings

1. **Locations are balanced.** Each of the 7 sites received about 14% of total volume, from Kakuma 2 (565,331 kg) to Kakuma 3 (534,998 kg).
2. **Nationalities are treated equitably.** Uganda received the most (514,112 kg) and Somalia the least (464,561 kg), a spread of about 10%.
3. **The food basket is standardized.** Super Cereal (666,645 kg) and Vegetable Oil (652,760 kg) led. Maize Flour, Beans, Rice, and Salt all fell between 635,000 and 650,000 kg.
4. **Volume is stable.** 2023: 1,294,168 kg, 2024: 1,288,664 kg, 2025: 1,282,557 kg, with no major seasonal spike or decline.
5. **Operations are the weak point.** Only 33.9% of distributions were completed, 33.3% were partial, and 32.9% were delayed.

## Recommendations

- Investigate the root causes of delays and partial completions (logistics, staffing, or supply).
- Keep the current equitable allocation across locations and nationalities.
- Monitor the commodity mix so it stays nutritionally balanced as the population changes.

## Tools

Microsoft Excel: PivotTables, PivotCharts, Slicers, `SUMIF`, `COUNTA`, `TEXT`, `YEAR`, `GETPIVOTDATA`, dashboard design

## Repository Contents

- `WFP_Food_Distribution_Kakuma_Kalobeyei_project_1.xlsx`: cleaned data, working sheet, pivot tables, and dashboard
- `WFP_Food_Distribution_Report.pdf`: summary report
- `dashboard.png`: dashboard screenshot

## Author

**Alek**, Data Analytics student, ARel Data Science Program
[www.linkedin.com/in/monicah-majok] | [https://github.com/majormonicahalek-gif]
