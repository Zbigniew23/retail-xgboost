# retail-xgboost

Predicting retail transaction revenue using XGBoost on transactional data with feature engineering for customer and time-based features.

# Online Retail Revenue Prediction

Project Overview

This project demonstrates a Machine Learning workflow for predicting revenue from an online retail dataset. The main goal was to explore data preprocessing, feature engineering, and model training using Linear Regression and XGBoost Regressor.

Dataset

- Source: https://www.kaggle.com/datasets/ishanshrivastava28/tata-online-retail-dataset

- Key features include: InvoiceDate, Country, UnitPrice, Quantity, CustomerId

- Target variable: Revenue = Quantity \* UnitPrice

# Data Preprocessing & Feature Engineering

- Converted InvoiceDate to datetime and extracted month, day, and weekday

- Calculated Revenue

- Removed negative quantities and prices

- Encoded categorical features (Country) using one-hot encoding

Models

1. Linear Regression

   - Baseline model

   - Achieved RMSE: 264.91, R²: 0.741

2. XGBoost Regressor

   - Model to compare with linear regression

   - Achieved RMSE: 282.3, R²: 0.706

   - Feature importance analyzed

# Results

- Linear Regression performed slightly better on this dataset compared to a simple XGBoost Regressor.
