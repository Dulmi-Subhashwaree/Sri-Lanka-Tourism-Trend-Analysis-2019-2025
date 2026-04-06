# 🌴 Analyzing Sri Lanka Tourism Trends and Major Event Impacts (2019–2025)

## Overview
This project analyzes tourist arrivals to Sri Lanka from 2019 to 2025
using real data from the Sri Lanka Tourism Development Authority.
The study examines how two major crises — the Easter Sunday Attacks
of April 2019 and the COVID-19 pandemic of 2020–2021 — disrupted
international tourism, and how Sri Lanka recovered to exceed
pre-crisis levels by 2024 and set a new all-time record in 2025.

The project follows a complete end-to-end data science workflow
using Python for data cleaning and analysis, and Power BI
for interactive dashboard visualization.

---

## Dataset
- **Source:** Sri Lanka Tourism Development Authority (SLTDA)
- **Format:** Excel (.xlsx) — 7 files, one per year
- **Number of records:** 16,068 rows (after cleaning)
- **Coverage:** 243 countries, January 2019 to December 2025
- **Columns:** Year, Month, Country, Number_of_Tourists, Date

---

## Project Components

### 1. Data Cleaning & Preparation (Python)
- Automated header detection across 7 differently formatted Excel files
- Month column mapping handling both full names and abbreviations
- Removal of separator rows, blank rows, and grand total rows
- Reshaping from wide format to long format using pandas melt()
- Standardization of country names to Title Case
- Removal of 180 duplicate rows
- Creation of Date column in YYYY-MM format

### 2. Exploratory Data Analysis (Python)
- Dataset structure and quality checks
- Annual arrivals summary and year on year comparison
- Top 10 tourist source countries identification
- Seasonal pattern analysis across all 7 years
- Sanity checks confirming COVID period accuracy

### 3. Event Impact Analysis (Python)
- Easter Sunday Attack impact measurement
  (before vs after comparison)
- COVID-19 impact analysis
  (2019 baseline vs 2020 and 2021)
- Recovery journey tracking
  (2022 to 2025 vs 2019 baseline)
- Percentage calculations for all event impacts

### 4. Power BI Dashboard
- 7 KPI cards — total arrivals, best year, worst year,
  Easter drop, COVID drop, 2024 recovery, 2025 growth
- Area chart — full 2019–2025 timeline with event markers
- Column bar chart — annual totals with color coding
- Donut chart — arrivals by world region
- Seasonality heatmap matrix — monthly patterns by year
- Recovery line chart — 2022–2025 vs 2019 baseline
- World map — arrivals by source country
- 3 interactive filters — Year, Country, Event Period
- DAX measures and calculated columns

---

## Key Findings

### 🐣 Easter Sunday Attacks — April 21, 2019
- Pre-attack monthly average: 246,867 arrivals
- May 2019 dropped to just 37,802 arrivals
- Impact: **-84.7%** vs pre-attack average
- Full recovery achieved within **6 months**

### 🦠 COVID-19 Pandemic — March 2020
- Borders closed March 2020
- Only **393 total arrivals** from April to December 2020
- Full year 2020: **-73.5%** vs 2019 baseline
- Full year 2021: **-89.8%** vs 2019 baseline
- Total lost arrivals: over **1.4 million**

### 📈 Recovery Journey — 2022 to 2025
| Year | Total Arrivals | Recovery vs 2019 |
|---|---|---|
| 2022 | 719,978 | 37.6% |
| 2023 | 1,487,303 | 77.7% |
| 2024 | 2,053,465 | ✅ 107.3% Full Recovery |
| 2025 | 2,362,521 | 🏆 123.5% New Record |

### 🌍 Market Insights
- India is the number one source market
  with 1,874,960 total arrivals over 7 years
- South Asia leads regionally at 33.6% market share
- Europe follows at 25% — UK, Russia, Germany, France
- Peak season: January, February, March, December
- Off-peak season: May, June, July (monsoon season)

---

## Limitations
- Dataset covers arrivals only — does not include
  tourist spending or length of stay
- Country name inconsistencies across years may have
  caused minor grouping errors
- Regional groupings in the donut chart are approximate
- 2025 data may include projected figures for later months

---

## Recommendations
- Diversify source markets beyond India to reduce
  single-market dependency
- Develop off-peak tourism products targeting
  European markets during monsoon months
- Use recovery patterns to plan infrastructure investment
  during future tourism downturns
- Monitor emerging markets like China and Middle East
  for future growth opportunities

---

## Challenges
- Each Excel file had a completely different structure
  requiring automated and robust parsing logic
- Circular dependency errors in Power BI DAX
  requiring Power Query solution for month sorting
- Balancing technical depth with clear visual storytelling
  for a non-technical audience

---

## Conclusion
This project demonstrates a complete end-to-end data science
workflow applied to a real-world dataset of national significance.

Sri Lanka's tourism sector showed remarkable resilience —
recovering from two unprecedented crises within 3 years
and setting a new all-time arrival record in 2025.

The combination of Python analysis and Power BI visualization
provides both technical depth and accessible insights
for data-driven tourism policy and planning decisions.

---

## Author
W.M. Dulmi Subhashwaree
Undergraduate
Bsc in Applied Data Science Communication 
---

## License
This project is for educational purposes only.
Data sourced from the Sri Lanka Tourism Development Authority
(SLTDA) annual statistical reports.
