# Global Tax Reform & Entrepreneurship Analysis

AI-driven analysis of how tax structures affect entrepreneurship across 196 countries using 43 years of World Bank data (1980–2022).

Completed as part of a Master of Business Analytics Capstone at Sunway University (May 2026).

## Key Results
- **XGBoost Regressor:** R² of 0.67 on unseen future years (2018–2022), a 177% improvement over the OLS baseline
- **Random Forest Classifier:** 74.8% accuracy predicting national income groups from tax data
- **Key finding:** Countries with a CIT-to-VAT ratio below ~0.23 show higher predicted business formation (SHAP threshold, stable across 20 model retrains)
- **Top driver:** Personal income tax had the largest SHAP impact on business entry
- Model captured the entrepreneurship declines during the 2008 Financial Crisis and COVID-19

Models were trained on 2017 and earlier and tested on 2018–2022, so each country's future is predicted from past data only.

## Live Dashboard
[Tax Response Engine](https://tax-response-engine.onrender.com): interactive policy simulator built with Gradio and Plotly (may take a minute to wake up).

## Tech Stack
Python, XGBoost, Random Forest, SHAP, Pandas, Scikit-learn, Gradio

## Files
| File | Description |
|---|---|
| `CodeFile_Data_Cleaning.ipynb` | Data wrangling & missing value imputation |
| `CodeFile_of_EDA_&_ML_Model.ipynb` | EDA, feature engineering & ML modelling |
| `Final_Clean_Dataset.xlsx` | Cleaned dataset |
| `Featured_Dataset.xlsx` | Dataset with engineered features used for modelling |
