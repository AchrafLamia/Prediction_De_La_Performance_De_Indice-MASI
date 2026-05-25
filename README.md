# Prediction De La Performance De L'Indice MASI

Prediction of the Moroccan All Shares Index (MASI) performance using machine learning and time-series forecasting techniques.

---

## Overview

This project applies machine learning methods to forecast the performance of the **MASI (Moroccan All Shares Index)**, the primary benchmark index of the **Casablanca Stock Exchange (Bourse de Casablanca)**. The goal is to build predictive models that can identify directional trends and estimate future index values based on historical market data and engineered financial features.

## Context

The **Casablanca Stock Exchange (CSE)** is the second largest stock exchange in Africa and the main financial market in Morocco. The MASI index aggregates all continuously quoted Moroccan equities and serves as the key indicator of the overall health and direction of the Moroccan capital market. Accurate forecasting of the MASI is of interest to institutional investors, portfolio managers, and financial analysts operating in the North African and broader MENA markets.

Predicting stock market indices is a challenging problem due to the non-stationary, noisy, and complex nature of financial time-series data. This project explores both traditional statistical machine learning approaches and, where applicable, deep learning architectures suited for sequential data.

## Project Structure

```
Prediction_De_La_Performance_De_Indice-MASI/
│
└── Predict_MASI_ .ipynb      # Main analysis and modeling notebook
```

## Methodology

### 1. Data Collection
- Historical MASI index price data (open, high, low, close, volume)
- Collection from publicly available financial data sources

### 2. Exploratory Data Analysis
- Visualization of historical index trends and volatility
- Statistical characterization of the time series (stationarity tests, autocorrelation analysis)

### 3. Feature Engineering
- Lag features and rolling window statistics (moving averages, rolling standard deviation)
- Technical indicators (RSI, MACD, Bollinger Bands, and similar momentum indicators)
- Return-based features and volatility proxies

### 4. Modeling
- Baseline models: Linear Regression, Ridge Regression
- Ensemble methods: Random Forest, Gradient Boosting (XGBoost / LightGBM)
- Recurrent architectures: LSTM (Long Short-Term Memory) for sequential pattern learning
- Train/validation/test split respecting temporal ordering to prevent data leakage

### 5. Evaluation
- Metrics: MAE, RMSE, MAPE, and directional accuracy
- Visual comparison of predicted vs. actual index values

## Tech Stack

| Category         | Tools / Libraries                              |
|------------------|------------------------------------------------|
| Language         | Python 3.x                                     |
| Data Handling    | Pandas, NumPy                                  |
| Visualization    | Matplotlib, Seaborn                            |
| Machine Learning | Scikit-learn, XGBoost / LightGBM               |
| Deep Learning    | TensorFlow / Keras (LSTM)                      |
| Notebook         | Jupyter Notebook                               |

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Prediction_De_La_Performance_De_Indice-MASI.git
   cd Prediction_De_La_Performance_De_Indice-MASI
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow
   ```

3. Open the notebook:
   ```bash
   jupyter notebook "Predict_MASI_ .ipynb"
   ```

## Notes

- All modeling steps follow a strict chronological train/test split to ensure no future data leaks into training.
- Financial forecasting models are exploratory and are not intended as investment advice.

## Author

**LAMIA ACHRAF**

---

*Casablanca Stock Exchange — Bourse de Casablanca | Moroccan Capital Markets | Time-Series Forecasting*
