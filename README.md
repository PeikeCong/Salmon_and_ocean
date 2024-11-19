# Predicting Salmon Attributes in Nova Scotia with Oceanic Variables

This project explores the relationship between salmon populations and oceanographic variables(temperature, salinity, current) to forecast salmon metrics (amount, length, and width) using time series modeling (SARIMA & Prophet). The work combines data preprocessing, exploratory analysis, and modeling to understand and predict how environmental changes impact salmon populations.

---

## Table of Contents  
1. [Introduction](#introduction)  
2. [Data Sources](#data-sources)  
3. [Preprocessing and Modeling](#preprocessing-and-modeling)  
4. [Usage](#usage)  
5. [Supplementary Materials](#supplementary-materials)  
6. [Clean Dataset](#clean-dataset)  

---

## Introduction  
Salmon are a vital part of coastal ecosystems and an indicator of marine biodiversity. This project leverages data-driven insights to understand how environmental changes, especially oceanographic conditions, affect salmon metrics over time.

The main components of the project include:  
- Combining data from different sources  
- Exploring relationships between variables  
- Applying and comparing time series forecasting models (e.g., SARIMA, Prophet)  
- Visualizing historical and predicted trends  

---

## Data Sources  

The datasets used for this project were sourced from open Canadian government repositories:  

- **Oceanographic Features**:  
  [Open Canada - Oceanographic Features](https://open.canada.ca/data/en/dataset/7da1f04f-49b0-4208-a49e-d0597b1f55c6)  

- **Salmon Hatchery Data**:  
  [Open Canada - Salmon Hatchery Data](https://ouvert.canada.ca/data/dataset/e2bc6ab0-eb87-e53d-1a7a-117df0433168)  

---

## Preprocessing and Modeling  

### Data Preprocessing  
The two datasets were combined to create a clean and structured dataset for modeling. Steps included:  
1. Handling missing values  
2. Standardizing timeframes  
3. Scaling and normalizing variables (e.g., temperature, salinity)  

### Time Series Models  
The following models were tested:  
- **SARIMA**: Seasonal Autoregressive Integrated Moving Average with exogenous variables (e.g., temperature, salinity)  
- **Prophet**: A robust forecasting tool suitable for seasonal patterns  

After comparison, the **SARIMA** and **Prophet** models were selected for final predictions based on their accuracy and interpretability.  

---

## Usage  

### Files  
1. **`ocean_forecast_v2.ipynb`**: Main notebook containing the preprocessing, exploratory analysis, and final modeling.  
2. **Supplementary Data and Code**:  
   - Additional notebooks and scripts for data combination and analysis of unused models.  

### Dependencies  
Install the required Python libraries before running the notebooks:  

```bash  
pip install pandas numpy matplotlib statsmodels fbprophet scikit-learn  
```  

### Running the Notebook  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-repo-name.git  
   ```  
2. Open the main notebook:  
   ```bash  
   jupyter notebook ocean_forecast_v2.ipynb  
   ```  
3. Follow the steps to reproduce the analysis and predictions.  

---

## Supplementary Materials  
- Additional models tested during the project (not included in final results)  
- Intermediate data combining steps  
- Exploratory visualizations  

These materials are provided in the `supplement_data` folder for reference.  

---

## Clean Dataset  
A preprocessed and clean dataset is included for direct usage. This dataset eliminates the need for redundant preprocessing steps.  

Location: `clean_data/clean_dataset.csv`  

---

Feel free to contribute to the project or raise issues for improvement! 😊  
