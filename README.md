# Wind Power Forecasting Using AI, ML, and Time-Series Techniques

This repository contains a complete framework for forecasting wind power output using artificial intelligence, machine learning, and traditional time-series modeling. The goal of this project is to develop accurate short-term and day-ahead forecasts that support renewable energy integration, grid reliability, and operational planning.

Wind generation is inherently variable due to atmospheric conditions. Accurate forecasting improves economic dispatch, reduces reserve requirements, and enables better scheduling for wind farm operators and utilities.

---

## Objectives

1. Apply data-driven machine learning and deep learning models to wind power forecasting.
2. Compare statistical time-series baselines with advanced neural architectures.
3. Build a flexible preprocessing pipeline for transforming raw wind data into model-ready inputs.
4. Evaluate model performance using industry-standard error metrics.
5. Provide reproducible code and structured workflows for research or deployment.

---

## Methodology Overview

### 1. Data Preprocessing
- Cleaning and handling missing data
- Temporal alignment of wind speed, direction, temperature, and pressure
- Normalization and scaling
- Lag features and rolling-window features
- Cyclical encoding for temporal variables (e.g., hour, month)

Scripts are located under `preprocessing/`.

### 2. Forecasting Models

This project investigates multiple model classes:

#### **Statistical Models**
- ARIMA / SARIMA  
- Exponential Smoothing
- Persistence (naïve) baseline

#### **Machine Learning Models**
- Random Forest Regressor  
- Gradient Boosting (XGBoost, LightGBM)

#### **Deep Learning Models**
- LSTM (Long Short-Term Memory networks)  
- GRU-based recurrent models  
- 1D CNN for temporal pattern extraction  
- Hybrid CNN-LSTM architectures  

Model implementations are included in the `models/` directory.

### 3. Evaluation

Performance metrics include:
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- Root Mean Squared Error (RMSE)
- Day-ahead vs short-term error comparison

Plots and detailed evaluation outputs are under `evaluation/` and `figures/`.

---
