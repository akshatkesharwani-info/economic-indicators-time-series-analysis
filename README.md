# 🌍 Economic Indicators Time Series Analysis


## Overview
An economic research firm wants to study 30 years of macroeconomic trends. This project analyzes GDP growth across major economies using time series decomposition, stationarity testing and ARIMA forecasting.

## Dataset
- World Economic Outlook 2022 — [Kaggle](https://www.kaggle.com/datasets/josephvm/world-economic-outlook-2022)

## Tech Stack
Python · Pandas · NumPy · Matplotlib · Seaborn · Statsmodels (ARIMA, ADF test, decomposition)

## Approach
1. Reshaped wide-format economic data (years as columns) into long format with `pd.melt`
2. Cleaned and converted Year/GDP_Growth fields to proper numeric types
3. Compared GDP growth across USA, China, India, Germany and Japan on a multi-line chart
4. Decomposed the USA GDP series into trend, seasonality and residual components
5. Ran an Augmented Dickey-Fuller (ADF) test to confirm stationarity before modeling
6. Fit an ARIMA(1,0,1) model and forecast USA GDP growth 5 years ahead
7. Computed descriptive statistics (mean, std, min, max) per country

## Key Results & Insights
- USA and China show the strongest GDP recovery post-2008 — China's growth consistently runs 6–10%
- India has the highest average growth rate (~6.5%) among the 5 major economies studied
- The ADF test confirms the USA GDP growth series is stationary (p < 0.05)
- The 2020 COVID shock is clearly visible — every country shows a sharp negative GDP growth spike
- The ARIMA model forecasts moderate USA growth of 2–3% over the next 5 years

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook economic_indicators_analysis.ipynb
```

## Project Structure
```
economic-indicators-time-series-analysis/
├── notebooks/economic_indicators_analysis.ipynb
├── images/  (gdp_comparison.png, decomposition.png, arima_forecast.png)
├── requirements.txt
└── README.md
```

## Author
Akshat Kesharwani — [LinkedIn](https://linkedin.com/in/akshat-kesharwani-b0452b346) · [Portfolio](https://akshatkesharwani-info.github.io)
