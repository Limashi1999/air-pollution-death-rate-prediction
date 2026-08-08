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
Raw Datasets
     ↓
Data Cleaning
     ↓
Data Transformation
     ↓
Dataset Merging
     ↓
Missing Value Handling
     ↓
Exploratory Data Analysis
     ↓
Outlier & Skewness Analysis
     ↓
Log Transformation
     ↓
Feature Preparation
     ↓
Time-Based Data Split
     ↓
 ┌───────────────────────┐
 │                       │
Regression           Classification
 │                       │
 ↓                       ↓
Model Training       K-Means
 │                       ↓
 ↓                  Risk Categories
Model Comparison        ↓
 │                  RF & KNN
 ↓                       ↓
XGBoost Selected     RandomForest Selected

## NOTE
The data_preparation.ipynb notebook performs the main data preparation and exploratory analysis.
The regression_analysis.ipynb notebook predicts the continuous DeathRate value.
The categorical_analysis.ipynb notebook performs the mortality risk classification task.

## Important
### Regression Analysis: 
Four regression models were trained and compared. Such as:

Linear Regression
Random Forest Regressor
KNN Regressor
XGBoost Regressor

The analysis includes:

Feature scaling
Feature importance analysis
Feature selection
Hyperparameter tuning
RandomizedSearchCV
TimeSeriesSplit
SHAP analysis
Residual analysis
Overfitting checks
Final model evaluation

### Classification Analysis:
K-Means clustering was first used to create mortality groups based on DeathRate. Four mortality risk categories were created:
0 → Low
1 → Moderate
2 → Elevated
3 → High

The classification task then used:

Random Forest Classifier
KNN Classifier

The classification analysis includes:

K-Means clustering
Elbow Method
Mortality risk category creation
Correlation analysis
Time-based train/validation/test split
GridSearchCV hyperparameter tuning
Classification reports
Confusion matrices

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
## 📁 Repository Structure

* **`data/`** 
* **`final_datasets/`** 
* **`models/`** 
* **`docs/`**


