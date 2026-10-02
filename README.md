# DS-201-Capstone-1
# Real Estate Investment Data Exploration

**Author:** Michael Barrera-Hernandez  
**Course:** DS 201  
**Data Source:** Federal Housing Finance Agency (FHFA) House Price Index

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Y_quw9y_8NWqbX0oFtF5lyme7r1yRP-m?usp=sharing)

## Project Overview

This project explores housing market trends using the Federal Housing Finance Agency (FHFA) House Price Index (HPI). The goal of the analysis is to understand the structure and contents of the dataset, examine housing price trends over time and across geographic regions, and consider how the data could be useful when evaluating potential real estate investments.

## 1. Understanding the Data

The FHFA House Price Index dataset contains information about changes in single-family home values across different geographic areas in the United States.

The dataset includes both monthly and quarterly observations. Quarterly data ranges from **1975 to 2026**, while monthly data ranges from **1991 to 2026**.

The dataset also provides broad geographic coverage, including:

- 410 Metropolitan Statistical Areas (MSAs)
- 51 state-level areas
- 10 U.S. or Census Division areas
- Puerto Rico

Important attributes include the geographic area, year, reporting period, type of House Price Index, seasonally adjusted HPI, and non-seasonally adjusted HPI.

## 2. Data Summary & Initial Insights

Summary statistics were calculated for the major numerical variables in the dataset, including the non-seasonally adjusted House Price Index (`index_nsa`), seasonally adjusted House Price Index (`index_sa`), and standard error (`rstderr`).

The non-seasonally adjusted HPI had a mean of approximately **199.98** and a median of **172.13**, while the seasonally adjusted HPI had a mean of approximately **216.69** and a median of **187.22**. The variation in these values demonstrates substantial differences in housing price trends across locations and time periods.

### Missing Values

Most variables contained no missing values. However:

- `index_sa` contained 89,897 missing values (48.33%).
- `rstderr` contained 127,801 missing values (68.70%).
- `note` contained 127,801 missing values (68.70%).

These observations were not automatically removed because some variables are only available or applicable for certain HPI series. The non-seasonally adjusted HPI (`index_nsa`) contains a value for every observation and serves as the primary measure used in the visual analysis.

### Housing Price Trends

The national House Price Index shows substantial long-term growth from 1991 to 2026. The index increased throughout much of the 1990s and early 2000s, declined following its mid-to-late-2000s peak, and recovered during the 2010s. Particularly rapid growth can be observed after 2020.

Regional comparisons also demonstrate that housing price trends differ across the nine U.S. Census Divisions. The Mountain Division experienced especially large increases in its House Price Index, while other regions followed different growth trajectories. These differences demonstrate the importance of considering geographic location when examining real estate markets.

## 3. Expanding Your Investment Knowledge

An additional dataset that could complement the FHFA House Price Index is the **Zillow Observed Rent Index (ZORI)**.

ZORI measures typical market rents across different geographic areas and tracks changes in rental prices over time. This information would be useful for evaluating real estate investments because property appreciation is not the only factor an investor may consider. Potential rental income can also influence the attractiveness of a real estate market.

The ZORI dataset complements the FHFA data by providing information about rental prices, while the FHFA House Price Index provides information about changes in home values. Comparing the two could provide a more complete picture of local real estate markets.

**Additional Dataset:** Zillow Observed Rent Index (ZORI) – Metro, All Homes + Multifamily, Smoothed, Monthly

**Dataset Link:**  
https://files.zillowstatic.com/research/public_csvs/zori/Metro_zori_uc_sfrcondomfr_sm_month.csv

## 4. Communicating the Findings

Overall, the analysis shows that U.S. housing prices have generally increased over the long term, although growth has not been consistent across every time period or geographic region. Housing markets can experience periods of growth, decline, and recovery, and different regions can experience substantially different price trends.

From an investment perspective, the results demonstrate why both **time and location** are important when examining real estate markets. However, an increase in home values alone does not necessarily indicate that a market is a good investment. Other factors, including rental income, affordability, and local market conditions, should also be considered.

## Data Sources

- **Federal Housing Finance Agency (FHFA) House Price Index:**  
  https://www.fhfa.gov/hpi/download/monthly/hpi_master.csv

- **Zillow Observed Rent Index (ZORI):**  
  https://files.zillowstatic.com/research/public_csvs/zori/Metro_zori_uc_sfrcondomfr_sm_month.csv
