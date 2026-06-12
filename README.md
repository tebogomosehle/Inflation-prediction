# Inflation-prediction
📈 Inflation Forecasting Using Time Series Models (ARIMA & Naive Benchmark)
📌 Project Overview

This project develops and compares multiple time series forecasting models to predict inflation (CPI) using South African macroeconomic data. The study focuses on evaluating whether advanced time series models (AutoARIMA and ARIMAX) outperform a simple persistence (naive) benchmark.

A key objective is to distinguish between statistical significance of predictors and actual forecasting performance.

📂 Dataset
📥 Data Sources

The dataset was constructed from macroeconomic indicators including CPI and selected explanatory variables (e.g. repo rate, money supply, and external economic indicators).

Key Variables
CPI (Inflation rate) – Target variable
CPI_lag (t−1) – Persistence benchmark feature
Repo rate – Monetary policy indicator
M3 Money Supply – Liquidity measure
External/US economic indicators – Global influence variables
Time Period

Monthly observations (approximately 2010–latest available year)

🛠️ Tools & Libraries
Python
Pandas
NumPy
Scikit-learn
Statsmodels
pmdarima (AutoARIMA)
Matplotlib
Seaborn
📊 Approach
Performed data cleaning and time series preprocessing
Created lagged CPI feature for persistence benchmarking
Split data into training and testing sets (time-based split)
Built baseline Naive (Persistence) model
Built AutoARIMA model (univariate)
Built AutoARIMAX model with exogenous variables
Evaluated models using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
Mean Absolute Percentage Error (MAPE)
Conducted residual diagnostics to test model adequacy
Compared forecasting performance against naive benchmark
🔍 Key Models
📌 Naive (Persistence) Model
Forecast: y
t
	​

=y
t−1
	​

Assumes inflation follows last observed value
Acts as baseline benchmark
📌 AutoARIMA (Univariate)
Automatically selects optimal (p, d, q) parameters
Captures autoregressive and moving average patterns
No external predictors included
📌 AutoARIMAX (With Exogenous Variables)
Includes macroeconomic predictors (repo rate, M3, etc.)
Tests whether external variables improve forecasting accuracy
📈 Results
Model	MAE	RMSE	MAPE
Naive (Persistence)	0.13	0.17	—
AutoARIMA	0.86	—	10.92%
AutoARIMAX	0.72	—	10.17%
⚠️ Key Findings
The naive persistence model outperformed AutoARIMA in raw error metrics
AutoARIMAX improved performance slightly over AutoARIMA
Predictor variables were statistically significant but did not strongly improve forecasting accuracy
Inflation exhibits strong short-term persistence
Complex models do not always outperform simple benchmarks in macroeconomic forecasting
💡 Key Insights
Statistical significance ≠ predictive power
Simple persistence models can be highly competitive in inflation forecasting
Macro variables may improve interpretability but not always accuracy
Model evaluation must always include a naive benchmark
Residual diagnostics confirm whether a model has captured all time-dependent structure
📊 Model Evaluation Strategy
Train-test split (time-based)
Benchmarking against naive forecast
Multi-metric evaluation (MAE, RMSE, MAPE)
Residual analysis (white noise assumption)
Comparative model performance analysis
🚀 Future Improvements
Incorporate SARIMAX with lagged macroeconomic variables
Test machine learning models (Random Forest, XGBoost)
Apply walk-forward validation for more robust evaluation
Explore structural break detection in inflation series
Feature engineering using lagged macroeconomic indicators
