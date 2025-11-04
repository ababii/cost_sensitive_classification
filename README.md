# Replication Package

## Overview

This replication package contains code and data for analyzing binary forecasting with asymmetric costs, including applications to recidivism prediction using the COMPAS dataset.

## Structure

- `code/` - Jupyter notebooks and R scripts
  - `data_cleaning.ipynb` - Data preprocessing and variable creation from COMPAS database
  - `empirical_application.ipynb` - LASSO-Logit and XGBoost models with symmetric/asymmetric classifiers
  - `simulations.ipynb` - Monte Carlo simulations comparing classification methods

- `data/` - Dataset files
  - `data_clean.csv` - Cleaned dataset for analysis

- `fig/` - Generated figures
- `tab/` - Generated tables

## Requirements

**Python packages:** numpy, pandas, matplotlib, scikit-learn, xgboost, tensorflow, keras, joblib

**R packages:** dplyr, pROC, xgboost, glmnet, caret, ggplot2, stargazer

## Key Results

The package generates:
- Tables 1-4 and Tables OA.1-OA.5 (simulation and empirical results)
- Figures 1, 3-7 and Figures OA.2 (asymmetric classification performance)

## Notes

- Data cleaning creates 780+ features from criminal history and demographics
- Empirical analysis uses 80-20 train-test split with 5-fold cross-validation
- Simulations use 1,000-10,000 observations with 1,000-5,000 Monte Carlo replications
- Computation time varies: simulations (~9-12 hours), empirical analysis (~2-4 hours)
