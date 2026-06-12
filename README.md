# Inflation-prediction
📈 Inflation Forecasting Using Time Series Models (ARIMA & Naive Benchmark)
# 📌 Project Overview

This project develops and compares multiple time series forecasting models to predict inflation (CPI) in South Africa, from 01 January 2010 until 01 December 2025. The project focuses on evaluating whether any advanced time series model (AutoARIMA) outperforms a simple persistence (naive) benchmark.

# 📂 Dataset and Data Sources
## 📥 Dataset
The dataset was constructed and compiled from macroeconomic indicators which include CPI, USDZAR exchange rates, Prime rates and Money Supply(M3). 
## Data Sources
CPI- South African Reserve Bank(SARB) website

M3- SARB website

Prime rates- SARB website

USDZAR exchange rates- Investing.com

# 🛠️ Tools & Libraries used
Python

Pandas

NumPy

Scikit-learn

Statsmodels

Matplotlib

Seaborn
# 📊 Approach
Performed data cleaning and time series preprocessing
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

# ⚠️ Key Findings
The naive persistence model outperformed AutoARIMA in raw error metrics
AutoARIMAX improved performance slightly over AutoARIMA
Predictor variables were statistically significant but did not strongly improve forecasting accuracy
Inflation exhibits strong short-term persistence
# 💡 Key Insights
Statistical significance ≠ predictive power
Simple persistence models can be highly competitive in inflation forecasting
Macro variables may improve interpretability but not always accuracy

# 🚀 Future Improvements
Incorporate SARIMAX with lagged macroeconomic variables
Test machine learning models (Random Forest, XGBoost)
Apply walk-forward validation for more robust evaluation

# 👤 Author
Tebogo Mosehle
📫 [tebogomosehle10@gmail.com]

Linkedin: www.linkedin.com/in/tebogo-mosehle-1806b319b
