# 📈 Time Series Forecasting for Portfolio Management Optimization

## Overview
This project focuses on applying **time series forecasting** and **statistical analysis** to enhance **portfolio management** strategies. By analyzing historical stock data and building predictive models, it enables **optimized asset allocation** and **better risk management** for a financial advisory firm, **Guide Me in Finance (GMF) Investments**.

The project covers:
- Data preprocessing & exploratory analysis
- Time series forecasting using ARIMA/SARIMA and LSTM
- Market trend analysis
- Portfolio optimization using Modern Portfolio Theory (MPT)
- Strategy backtesting against a benchmark

---

## 📌 Business Objective
**GMF Investments** specializes in personalized portfolio management.  
Using **data-driven insights**, the firm predicts market trends and optimizes asset allocation to help clients:
- Minimize risks
- Capitalize on market opportunities
- Achieve their financial objectives

As a Financial Analyst at GMF, your role is to:
- Apply time series forecasting to historical financial data
- Use insights to optimize a portfolio of stocks and ETFs
- Backtest strategies to validate performance

---

## 📊 Data Sources
Historical financial data (2015-01-01 to 2024-10-31) sourced from **Yahoo Finance** using `yfinance`.

### Assets:
- **TSLA** (Tesla) – High-growth, high-risk consumer discretionary stock
- **BND** (Vanguard Total Bond Market ETF) – Stability, low risk
- **SPY** (S&P 500 ETF) – Diversified, moderate risk

### Data Includes:
- Date
- Open, High, Low, Close (Adjusted Close)
- Volume
- Volatility (calculated in analysis)

---

## 📂 Project Structure
- ├── .vscode/
- │ └── settings.json
- ├── .github/
- │ └── workflows/
- │ └── unittests.yml
- ├── src/
- │ └── init.py
- ├── notebooks/
- │ ├── init.py
- │ └── Preprocess_and_Explore_the_Data.ipynb
- ├── data/
- ├── tests/
- │ └── init.py
- ├── scripts/
- │ ├── init.py
- │ ├── EDA.py
- │ └── README.md
- ├── .gitignore
- ├── requirements.txt
- ├── README.md

---

## 🛠 Installation
Clone the repository:
```bash
git clone https://github.com/ElbetelTaye/Time-Series-Forecasting-for-Portfolio-Management-Optimization-.git
cd Time-Series-Forecasting-for-Portfolio-Management-Optimization
Install dependencies:

pip install -r requirements.txt
```


🚀 Usage
- Run the preprocessing and EDA:

- jupyter notebook notebooks/Preprocess_and_Explore_the_Data.ipynb
# Scripts are modular:

- EDA.py – Data loading, cleaning, and visualization

- Functions can be applied to individual assets or run sequentially for all

## 📋 Project Workflow
## Task 1: Preprocess and Explore the Data
- Load historical data for TSLA, BND, SPY.

- Handle missing values (forward/backward fill).

- Check data types and statistics.

# EDA:

- Closing price trends

- Daily volatility (returns)

- Rolling mean & std

- Outlier detection (Z-score)

- Seasonality & trend decomposition

- Risk metrics: Value at Risk (VaR), Sharpe Ratio

- Autocorrelation (ACF/PACF) analysis

## Task 2: Develop Time Series Forecasting Models
# Models Implemented:

- ARIMA / SARIMA (statistical)

- LSTM (deep learning)

- Chronological train/test split

- Parameter tuning:

- ARIMA: auto_arima / grid search

- LSTM: layers, neurons, epochs, batch size

- Evaluate using MAE, RMSE, MAPE

## Task 3: Forecast Future Market Trends
- Forecast next 6–12 months for TSLA.
- Include confidence intervals.
- Analyze:
- Long-term trends
- Volatility & risk from CI width
- Market opportunities & risks

## Task 4: Optimize Portfolio Based on Forecast
# Expected returns:

- TSLA: forecasted returns

- BND & SPY: historical annualized returns

- Covariance matrix from returns

- Generate Efficient Frontier:

- Max Sharpe Ratio portfolio

- Min Volatility portfolio

- Final recommendation:

- Asset weights

- Expected return, volatility, Sharpe Ratio

## Task 5: Strategy Backtesting
- Period: Aug 2024 – Jul 2025

- Benchmark: 60% SPY / 40% BND

- Simulate:

- Hold optimal weights or rebalance monthly

- Compare:

- Cumulative returns

- Sharpe Ratios

- Total returns