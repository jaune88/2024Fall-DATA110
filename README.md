# 2024Fall-DATA110
# Predicting and Understanding Risk Factors of Diabetes

## Project Overview
This project uses CDC  data to identify top risk factors for diabetes using classification models. We focused on predicting diabetes status and understanding which features—like blood pressure, BMI, and general health—correlate most strongly with the disease.

## Data
- Source: [CDC Dataset](https://www.cdc.gov/brfss/annual_data/annual_2015.html)
- 253,680 samples, 21 features
- Cleaned for balance and outliers; prediabetic cases removed

## Methods
- Models: **Decision Tree Classifier** (with and without feature selection), **Random Forest** for comparison
- Custom feature selection algorithm: tested 1,000 random combinations of 5 features
- Evaluation: train/test split (80/20), accuracy comparison

## Key Findings
- **HighBP**, **BMI**, and **GenHlth** were the most predictive features
- **Physical activity** was *not* a strong predictor despite our original hypothesis
- Random forest slightly outperformed decision tree (0.73 vs 0.715 test accuracy), but lacked interpretability

## Limitations
- Model is not for diagnosis and does not establish causation
- Should be used by professionals as a screening aid, not as a standalone diagnostic tool
