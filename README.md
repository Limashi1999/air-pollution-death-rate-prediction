# Air Pollution Death Rate Prediction and Risk Classification

An end-to-end machine learning project that predicts air pollution-related death rates and classifies countries into different mortality risk levels using environmental, population, and healthcare-related data.

## Project Overview

Air pollution is an important environmental and public health issue that can contribute to increased mortality. This project uses machine learning to study the relationship between air pollution, population, healthcare availability, and air pollution-related death rates.

The project has two main objectives:
1. Predict the numerical air pollution-related death rate using regression models.
2. Classify countries into mortality risk categories using classification models.

The project combines data from NASA AQDH, WHO and the World Bank and applies data preparation, exploratory data analysis, regression, classification, feature analysis, and model evaluation.

## Datasets
NASA Earthdata / SEDAC — Country Trends in Major Air Pollutants (AQDH)
World Health Organization (WHO) — Ambient Air Pollution Attributable Death Rate
World Bank — Hospital Beds per 1,000 People

## Machine Learning Workflow

1. **Raw Datasets**
2. **Data Cleaning**
3. **Data Transformation**
4. **Dataset Merging**
5. **Missing Value Handling**
6. **Exploratory Data Analysis (EDA)**
7. **Outlier and Skewness Analysis**
8. **Log Transformation**
9. **Feature Preparation**
10. **Time-Based Data Split**

### Regression

* Model Training
* Model Comparison
* **XGBoost Selected**

### Classification

* K-Means Clustering
* Risk Category Creation
* Random Forest and KNN Model Training
* **Random Forest Selected**

**Data Preparation → EDA → Feature Preparation → Time-Based Split → Regression & Classification → Model Comparison → Best Model Selection**

## NOTE
The data_preparation.ipynb notebook performs the main data preparation and exploratory analysis.
The regression_analysis.ipynb notebook predicts the continuous DeathRate value.
The categorical_analysis.ipynb notebook performs the mortality risk classification task.

## Key Output Files
Source and cleaned datasets
  air_pollutant_dataset_CLEANED.csv
  death_rates_dataset_CLEANED.csv
  hospital_beds_dataset_CLEANED.csv
  
Processed datasets
  final_raw_dataset.csv
  log_transformed_dataset(with-null-values).csv
  log_transformed_dataset(without-null-values).csv
  log_transformed_dataset(without-null-values)_categorical.csv

## Repository Structure

* **`data/`** 
* **`final_datasets/`** 
* **`models/`** 
* **`docs/`**


