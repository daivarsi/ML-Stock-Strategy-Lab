# 📈 Stock Price Prediction with SVR and XGBoost

This project compares two advanced regression models — **Support Vector Regression (SVR)** and **XGBoost** — to predict Tesla (TSLA) stock prices based on recent historical data. The goal is to move beyond oversimplified linear regression and evaluate how more powerful, nonlinear models perform on real financial time series data.

---

## 🔍 Project Overview

- **Data Source**: Yahoo Finance (via `yfinance`)
- **Models Used**: SVR (RBF Kernel), XGBoost Regressor
- **Evaluation Metrics**: Mean Squared Error (MSE), R² Score
- **Time Window**: Last 90 days of TSLA closing price data

---

## 🧰 Technologies Used

- Python 3.10+
- scikit-learn
- xgboost
- yfinance
- matplotlib, pandas, numpy

---

## 📦 Installation

Run the following in a Google Colab cell or your terminal:

```bash
pip install yfinance xgboost scikit-learn
