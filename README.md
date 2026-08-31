# Air Quality Index (AQI) Prediction Using Machine Learning

## Project Overview

A predictive analytics project that analyzes historical air quality data from Chennai and forecasts future Air Quality Index (AQI) values using machine learning.

## Objective

- Analyze historical AQI trends
- Engineer time-based and historical pollution features
- Build AQI prediction models
- Compare different regression algorithms
- Forecast AQI for 30 future days
- Classify predicted AQI into air-quality categories

## Dataset

- **Dataset:** Air Quality Data in India
- **Source:** Kaggle
- **City:** Chennai
- **Period:** 2015–2024
- **Frequency:** Daily
- **Target:** AQI
- **Original Records:** 3,653
- **Modeling Records:** 3,623

## Models Used

- Linear Regression
- Random Forest
- Gradient Boosting

## Model Performance

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 128.49 | 147.96 | -0.0269 |
| **Random Forest** | **127.45** | **146.68** | **-0.0093** |
| Gradient Boosting | 128.52 | 148.72 | -0.0375 |

**Selected Model: Random Forest**

Random Forest achieved the best performance on the unseen test dataset.

## 30-Day AQI Forecast

Forecast period: **January 1, 2025 – January 30, 2025**

- Average predicted AQI: **247.42**
- Minimum predicted AQI: **220.80**
- Maximum predicted AQI: **272.81**
- Poor AQI days: **30/30**

## Key Insights

- Historical AQI showed substantial daily variation.
- Severe was the most frequent historical AQI category.
- Historical AQI and lagged pollutant values were important model features.
- Random Forest performed best among the evaluated models.
- The test R² was close to zero, indicating limited ability to explain daily AQI variation.

## Technologies

Python • Pandas • NumPy • Matplotlib • Scikit-learn • Google Colab

## Project Files

- `Air_Quality_Predictive_Analytics.ipynb` — Complete analysis and ML workflow
- `chennai_aqi_30_day_forecast.csv` — 30-day AQI predictions
- `model_test_results.csv` — Model evaluation results
- `feature_importance.csv` — Feature importance results


This project demonstrates an end-to-end predictive analytics workflow for AQI forecasting, including data preprocessing, exploratory analysis, feature engineering, machine learning, model evaluation, feature importance analysis, and future forecasting.
