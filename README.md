# 🐟 Predicting Salmon Attributes in Nova Scotia with Oceanic Variables

## Overview  
This is a project dedicated to understanding and predicting salmon attributes in Nova Scotia using oceanographic and hatchery data. Through data analysis and modeling, this project aim to explore how environmental factors affect salmon populations and provide insights for conservation and sustainable practices.  

---

## Project Motivation  

Wild Atlantic salmon are vital to Nova Scotia's ecosystem, economy, and culture, particularly for Indigenous communities, where they hold spiritual significance. However, their populations have declined dramatically due to environmental changes, making them a critical indicator of coastal ecosystem health.  

This project addresses the urgent need to analyze long-term data and predict future trends, offering actionable insights for recovery and resilience.  

---

## Data Sources  

### Oceanographic Data  
- **Dataset**: [Northwest Atlantic Oceanographic Features](https://open.canada.ca/data/en/dataset/7da1f04f-49b0-4208-a49e-d0597b1f55c6)  
- **Content**: The Ocean Data Inventory database is an inventory of all of the oceanographic time series data held by the Ocean Science Division at the Bedford Institute of Oceanography. The data archive includes about 5800 current meter and acoustic doppler time series, 4500 coastal temperature time series from thermographs, as well as a small number (200) of tide gauges. Many of the current meters also have temperature and salinity sensors. The area for which there are data is roughly defined as the North Atlantic and Arctic from 30° - 82° N, although there are some minor amounts of data from other parts of the world. The time period is from 1960 to present. The database is updated on a regular basis.
### Salmon Hatchery Data  
- **Dataset**: [Nova Scotia Fish Hatchery Stocking Records](https://ouvert.canada.ca/data/dataset/e2bc6ab0-eb87-e53d-1a7a-117df0433168) 
- **Content**: Fish stocking records from Nova Scotia fish hatcheries. Includes trout and salmon stocking, size, number, location, stock and growth stage. Records contain both fall and spring distributions. 

---

## Process  

### 1. **Data Preprocessing**  
- Combined and cleaned datasets to align time frames and variables.  
- Removed outliers and standardized variables for consistent analysis.  
- Prepared clean datasets for modeling and visualization.  

### 2. **Visualization and Insights**  
- **Trend Analysis**: Observed increasing volatility in environmental variables over time and a steady decline in salmon numbers.  
- **Correlation Analysis**: Identified strong relationships between fish length/width and oceanographic variables.  

### 3. **Modeling**  
Tested six time-series models to predict salmon attributes, focusing on the two best-performing methods:  
- **Prophet**: Used for population prediction, excelling without external variables.  
- **SARIMA**: Applied to predict length and width, incorporating temperature, salinity, and currents for enhanced accuracy.  

### 4. **Key Findings**  
- Low salmon length and width observed in January, with a sharp decline in February.  
- Predictions suggest challenges with parr survival in post-spawning seasons.  
- Models provide early warnings, highlighting resilience thresholds.  

---

## Recommendations  

To support salmon recovery and resilience:  
1. **Enhance Habitat Restoration**: Protect and improve spawning grounds.  
2. **Promote Sustainable Fishing**: Reduce quotas and adopt selective fishing gear.  
3. **Monitor Environmental Impact**: Track changes in temperature, salinity, and other key variables.  
4. **Adopt Climate Mitigation Strategies**: Address cascading effects of warming oceans.  

---

### Current Limitations and Potential Improvements  

- **Geographical Context**: The analysis does not incorporate geographical data or detailed fish habitat information, which could enhance the precision of predictions.  
- **Biological and Ecological Factors**: Factors such as fish growth stages and interactions with closely connected species were not included, limiting a holistic understanding of the ecosystem dynamics.  
- **Data Recency**: The datasets only extend up to 2016, making the results a methodological demonstration rather than directly applicable to current conditions (2024).  

Future iterations could address these limitations by integrating more comprehensive datasets and real-time monitoring to improve the model's accuracy and relevance.  

---  

## Repository Structure  

```
📂 project-root  
├── 📂 data  
│   ├── oceanographic_cleaned.csv  
│   ├── salmon_hatchery_cleaned.csv
│   ├── salmon_hatchery_cleaned.csv  
├── 📂 notebooks  
│   ├── ocean_forecast_v2.ipynb  # Main modeling and prediction notebook  
│   ├── supplement_models.ipynb # Alternative models and additional analyses  
├── 📂 visualizations   
└── 📜 README.md  # Project documentation (this file)  
  
```  

---

## Acknowledgments  

This project leverages publicly available datasets provided by the Government of Canada. 
We hope this project inspires further research and action for the conservation of salmon and coastle ecosystems. 
