[![Status](https://img.shields.io/badge/status-complete-brightgreen?style=flat-square)](https://github.com)
[![Python](https://img.shields.io/badge/python-3.8+-blue.svg?style=flat-square)](https://www.python.org)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-ffffff?logo=python&logoColor=blue)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Maps-3F4F75?logo=plotly&logoColor=white)
# PRODIGY_DS__-01
--
**Author:** Adeyeye Blessing Temidayo  
**CIN:** PIT/DEC25/10676
---
# World Bank Population Analysis (1960-2024)

## 📌 Project Overview
A comprehensive analysis of global population trends using World Bank Development Indicators, examining demographic shifts across 217 countries from 1960 to 2024.
This project analyzes 65 years of population data to uncover global demographic patterns, regional disparities, and economic-demographic relationships. The analysis reveals that global population has grown from 3 billion to 8 billion, with significant variations across income groups and regions.

### Key Findings

- **Average country growth:** 217.8% over 65 years (median: 164.3%)
- **Regional leader:** Asia contains 59% of global population (4.7 billion)
- **Income correlation:** Low-income countries grew 312% vs. 78% for high-income nations
- **Fastest growers:** UAE (9,825%), Qatar (4,687%), Kuwait (987%)
- **Recent trends:** Growth deceleration in developed nations, continued expansion in Sub-Saharan Africa

---

## 📊 Dataset

- **Source:** World Bank Development Indicators
- **Indicator:** Total Population (SP.POP.TOTL)
- **Coverage:** 217 countries/territories, 1960-2024
- **Records:** 17,289 country-year observations after preprocessing

---

## Methodology

### 1. Data Preparation
- Merged population data with regional and income group metadata
- Reshaped from wide to long format for time-series analysis
- Handled missing values: median imputation for population, case deletion for metadata

### 2. Growth Calculations
Computed multiple growth metrics:
- **Year-over-Year (YoY):** Annual percentage changes
- **Decadal Growth:** 10-year period comparisons (1960-1970, 1970-1980, etc.)
- **Total Growth:** Overall change from 1960 to 2024
- **CAGR:** Compound annual growth rate over 64 years

### 3. Comparative Analysis
- Regional aggregations and trends
- Income group stratification
- Country rankings (fastest/slowest growth, top populations)

### 4. Visualizations
- Regional population distribution charts
- Time-series growth trends (log scale)
- Growth distribution histograms
- Income group boxplots
- Interactive choropleth world map

---

##🧰 Technologies

- **Python 3.13** - Core programming language
- **pandas** - Data manipulation and transformation
- **NumPy** - Numerical computations
- **Matplotlib & Seaborn** - Static visualizations
- **Plotly** - Interactive maps and charts

---

## 💻 Installation

```bash
# Clone the repository
git clone <https://github.com/Temidayo23/PRODIGY_DS__-01>
cd world-bank-population-analysis

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook world_bank_Data_Analysed.ipynb

```

## 📂 Project Structure

```
├── world_bank_Data_Analysed.ipynb    # Main analysis notebook
├── README.md                         # This file
├── requirements.txt                  # Python dependencies
├── data/
│   ├── API_SP.POP.TOTL_DS2_en_excel_v2_61.xls
│   └── Metadata_Country_API_SP.POP.TOTL_DS2_en_csv_v2_38144.csv
└── visualizations/
    ├── top10_growth.png
    └── Distribution_of_Total_population_Growth_Rates.png
```

## Results Highlights

### Regional Distribution (2024)
| Region | Population | % of Global |
|:-------|:-----------|:------------|
| Asia | 4.7 billion | 59% |
| Africa | 1.4 billion | 18% |
| Europe | 745 million | 9% |
| Latin America | 659 million | 8% |
| North America | 375 million | 5% |

### Growth by Income Group (1960-2024)
| Income Level | Median Growth | Range |
|:-------------|:--------------|:------|
| Low income | 312% | 150-980% |
| Lower-middle | 203% | 85-650% |
| Upper-middle | 142% | -15-520% |
| High income | 78% | -30-290% |

### Selected Countries
- **India:** 283% growth (1960: 450M → 2024: 1.43B) - Now world's most populous
- **China:** 117% growth (1960: 667M → 2024: 1.45B)
- **Nigeria:** 447% growth (1960: 45M → 2024: 229M) - Africa's largest
- **United States:** 85% growth (1960: 180M → 2024: 335M)

## 📊Visualizations

The project includes both static and interactive visualizations:

1. **Regional Population Bar Chart** - 2024 distribution
2. **Multi-line Time Series** - Regional trends (log scale)
3. **Top 10 Growth Chart** - Fastest growing countries
4. **Distribution Histogram** - Growth rate patterns with KDE
5. **Income Group Boxplots** - Growth by economic classification
6. **Interactive Choropleth Map** - Global growth visualization with hover details

<table>
    <tr>
        <img src="figures/Total Population by Region (2024).png" width="400" />
        <img src="figures/Top 10 Fastest Growing Countries (1960-2024).png" width="400" />
        <img src="figures/Population Growth Trends by Region (1960-2024).png" width="400" />
        <img src="figures/Population Growth Distribution by Income Group (1960-2024).png" width="400" />
        <img src="figures/Distribution of Growth Rates by Region.png" width="400" /> 
    </tr>
</table>

## ⚠️ Limitations

- Analysis limited to population totals; age structure and demographic composition not examined
- Some countries have incomplete temporal coverage
- Missing data addressed through median imputation (3.5% of records)
- Descriptive analysis; causal relationships not established
- Recent years (2020-2024) may have higher data uncertainty

## 🚀 Future Work

- [ ] Integrate additional indicators (fertility, mortality, life expectancy)
- [ ] Implement time-series forecasting (ARIMA, Prophet)
- [ ] Develop interactive Streamlit dashboard
- [ ] Add subnational analysis where data available
- [ ] Perform clustering analysis to identify demographic typologies
- [ ] Connect to World Bank API for real-time updates

## 📧 Contact
Adeyeye Blessing Temidayo (adeyeyeblessing2017@gmail.com) Feel free to reach out for collaborations or questions regarding this analysis!

## 📄 License
MIT License Copyright (c) 2026 Adeyeye Blessing Temidayo

Permission is hereby granted, free of charge... (See full text in repository)

Disclaimer: This project was developed as part of a Data Science project with Prodigy InfoTech and uses the Kaggle Twitter Entity Sentiment Analysis Dataset.


