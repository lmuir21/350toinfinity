# Codebook for `epi_top15.csv` Dataset

This codebook describes each variable included in the dataset `epi_top15.csv`, which was used for the analysis of education and economic growth trends among the 15 most populous countries (2000–2022).

## Table of Contents
1. [Overview](#overview)
2. [Variables](#variables)
3. [Notes](#notes)

---

## Overview

- **Dataset Name**: `epi_top15.csv`
- **Number of Rows**: 345 (15 countries × ~23 years each)
- **Number of Columns**: 14
- **Time Period**: 2000–2022
- **Geographic Scope**: 15 most populous countries
- **Purpose**: Analyze trends in education enrollment and economic growth.

---

## Variables

| Variable                  | Description                                              | Unit / Notes                     | Data Type      |
|---------------------------|----------------------------------------------------------|-----------------------------------|----------------|
| `country`                 | Country ISO 3-letter code (e.g., USA, IND, CHN)          | Categorical (3-letter code)      | Categorical    |
| `year`                    | Calendar year                                            | Integer (2000–2022)              | Integer        |
| `GDP_per_capita`          | GDP per capita (constant 2015 USD)                       | USD                              | Numeric        |
| `GDP_growth`              | Annual GDP growth rate                                   | Percentage (%)                   | Numeric        |
| `Primary_enrollment`      | Gross enrollment in primary education                    | Percentage (%)                   | Numeric        |
| `Secondary_enrollment`    | Gross enrollment in secondary education                  | Percentage (%)                   | Numeric        |
| `Tertiary_enrollment`     | Gross enrollment in tertiary education                   | Percentage (%)                   | Numeric        |
| `Education_expenditure`   | Government education expenditure as % of GDP            | Percentage (%)                   | Numeric        |
| `Population`              | Total national population                                | Number of people                 | Numeric        |
| `YoY_GDP_per_capita`      | Year-over-year % change in GDP per capita                | Percentage (%)                   | Numeric        |
| `YoY_Primary_enrollment`  | Year-over-year % change in primary enrollment            | Percentage (%)                   | Numeric        |
| `YoY_Secondary_enrollment`| Year-over-year % change in secondary enrollment          | Percentage (%)                   | Numeric        |
| `YoY_Tertiary_enrollment` | Year-over-year % change in tertiary enrollment           | Percentage (%)                   | Numeric        |
| `Education_Progress_Index`| Composite education progress score (via PCA)            | Standardized index (unitless)    | Numeric        |

---

## Notes

1. **Missing Data**:
   - Missing values for enrollment rates were imputed using the column mean before performing PCA.
   - Other missing values were left as-is.

2. **Derived Variables**:
   - `YoY_GDP_per_capita`, `YoY_Primary_enrollment`, `YoY_Secondary_enrollment`, and `YoY_Tertiary_enrollment` were calculated as year-over-year percentage changes.
   - `Education_Progress_Index` was derived using Principal Component Analysis (PCA) to summarize progress across all education levels.

3. **Units**:
   - GDP-related columns are in constant 2015 USD.
   - Enrollment ratios and growth rates are percentages.
   - Population is in absolute numbers.

---

*Codebook created on: 4/28/2025*  
*Authors: Daisy Cossio, Iliyan Sherali, Liane Muir*
