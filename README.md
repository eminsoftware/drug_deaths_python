# Trends in Accidental Drug-Related Deaths (2012-2024)

**Project Level**: Intermediate to Advanced

## Overview

This project is an in-depth exploratory data analysis (EDA) and cleaning exercise focusing on accidental drug-related deaths between 2012 and 2024. The primary goal was to uncover key demographic, geographical, and temporal trends, and to identify the substances most frequently contributing to fatalities.

The analysis utilizes the power of the **Pandas** library for data manipulation and preparation, transforming raw, inconsistent public health data into actionable insights that can inform public health strategies and resource allocation.

## Project Breakdown

The analysis was performed in a structured Jupyter Notebook workflow, divided into the following key phases:

### 1. Data Acquisition and Setup
* Loaded the `Accidental_Drug_Related_Deaths_2012-2024.csv` dataset.
* Configured Pandas display settings to ensure visibility of all columns for thorough inspection.

### 2. Data Cleaning and Preprocessing
The raw dataset required extensive cleaning to ensure data quality and consistency:
* **Case Standardization**: Applied a capitalization function to ensure uniform casing across categorical columns (e.g., `Race`, `Location`, `County`).
* **Ethnicity Normalization**: Addressed the highly inconsistent `Ethnicity` column by creating a new, standardized column (`Hispanic/Latino` vs. `Non-Hispanic/Latino`).
* **Data Type Conversion**: Converted the `Date` column to the `datetime` format to enable robust temporal analysis.
* **Feature Engineering**: Extracted the year from the `Date` column for time-series aggregation.
* **Redundancy Reduction**: Dropped non-usable or redundant geographic columns (e.g., `ResidenceCityGeo`, `InjuryCityGeo`).
* **Duplication Check**: Verified and confirmed the absence of duplicate rows.

### 3. Exploratory Data Analysis (EDA)

* **Temporal Trend Analysis**: Grouped data by year to analyze the trend of accidental deaths over the 2012–2024 period.
* **Substance Analysis**: Identified the most frequently listed primary `Cause of Death` entries (e.g., Fentanyl, Cocaine, Heroin).
* **Demographic Segmentation**:
    * Calculated total counts by `Sex` and identified the ratio of male-to-female fatalities.
    * Aggregated deaths by `Race` to identify the most affected populations.
    * Calculated the average age of victims, segmented by county and gender.
* **Geographical Analysis**: Determined the counties with the highest incidence of accidental drug-related deaths.

## Data Source

| **Dataset** | `Accidental_Drug_Related_Deaths_2012-2024.csv` | Dataset of accidental drug-related deaths in Connecticut from 2012 to 2024. |
| **Source URL** | (https://catalog.data.gov/dataset/accidental-drug-related-deaths-2012-2018) |

## Conclusion

The analysis provided clear, data-driven insights into the nature of the drug fatality crisis in the studied region:

1.  **Fentanyl Dominance:** Acute Fentanyl Intoxication was the single most common cause of death, confirming its central role in the opioid crisis during this period.
2.  **Worsening Temporal Trend:** The total number of accidental deaths demonstrated a significant upward trajectory, peaking dramatically around 2021 before slightly leveling off.
3.  **Significant Gender Disparity:** The data revealed a substantial gender skew, with **Male** individuals accounting for the overwhelming majority (approx. 74%) of accidental drug-related fatalities.

---
