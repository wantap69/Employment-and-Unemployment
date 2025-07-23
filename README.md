# Sectoral Analysis of Employment in Metro Manila Using PSA’s LFS Data

## 📄 Overview

This project analyzes employment and unemployment trends in the **National Capital Region (NCR)** using data from the **Philippine Statistics Authority's Labor Force Survey (LFS)** for **March 2024**. The analysis focuses on:
- Distribution of the workforce across **major sectors** (Agriculture, Industry, Services)
- Breakdown by **sub-industries**
- **Normality testing** of employment weights
- Visualization of weighted and unweighted frequencies
- Initial insights into which sectors dominate NCR's labor force

## 📁 File Contents

- `ncr_employment.html`: An interactive HTML document generated from an R Markdown or Quarto script. It contains:
  - **Data Cleaning steps**
  - **Variable transformation** and recoding (e.g., major/sub-sector, employment status)
  - **Exploratory Data Analysis (EDA)**
  - **Normality testing** using Shapiro–Francia Test (`sf.test`)
  - **Plots and tables** for employment frequency and distribution

## 🧪 Methodology

- **Dataset Source**: PSA's LFS data downloaded from [psada.gov.ph](https://psada.psa.gov.ph/catalog/LFS/about)
- **Tools Used**:
  - `tidyverse`: For data wrangling and visualization
  - `nortest`: For normality testing
  - `pander`: For generating APA-style tables
  - `here`: For relative file path management

- **Key Variables**:
  - `PUFC15_PKB`: Industry classification (used to derive major and sub-sectors)
  - `PUFREG`: Region (filtered for NCR only)
  - `PUFC09_WORK`: Employment status (employed/unemployed)
  - `PUFC07_GRADE`: Educational attainment
  - `PUFWGTPRV`: Final sampling weight (used for population estimation)

## 📊 Highlights from the Report

- The **Services sector** overwhelmingly dominates NCR employment.
- The **Industry sector** is second, while **Agriculture** accounts for the smallest portion.
- **Weighted population estimates** and **raw frequencies** were both analyzed.
- **Normality tests** suggest that employment weights in Industry and Services are **not normally distributed**, supporting the use of **log transformation** in further modeling.


## 👤 Author

**Benedict Bautista**  
Bulacan State University
BS in Applied Statistics — Philippines

## 🔗 References

- [Philippine Statistics Authority LFS Catalog](https://psada.psa.gov.ph/catalog/LFS/about)
- PSA Labor Force Survey — March 2024

---

