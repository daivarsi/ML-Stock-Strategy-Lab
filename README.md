# 📊 ML Stock Strategy Lab

An evolving, modular project exploring machine learning and deep learning techniques for forecasting stock price trends and simulating trading strategies. Using real market data and powerful models, each module investigates a different question in quantitative finance and time-series prediction.

---

## 🔍 Objective
**Can machine learning not only predict financial movements but also drive profitable decisions?**

From SVR to XGBoost to LSTMs and full backtests, this lab walks through both modeling and deploying ML strategies in trading contexts.

---

## 🧱 Repository Structure

```
ml-stock-strategy-lab/
├── baseline_svr_xgboost/            # 🔹 Baseline regression using SVR + XGBoost
│   └── tesla_price_regression.ipynb
├── technical_features/             # 🔹 Add moving averages, RSI, volume, MACD, etc.
│   └── feature_engineered_model.ipynb
├── classification_movement/        # 🔹 Predict direction (Up/Down) and backtest strategy
│   └── direction_classifier_with_backtest.ipynb
├── deep_learning_lstm/             # 🔹 LSTM for time-series forecasting
│   └── lstm_price_forecast.ipynb
├── backtesting_trades/             # 🔹 (optional) Separated strategy notebooks if modularized
│   └── strategy_backtest.ipynb
├── crypto_modeling/                # 🔹 Compare crypto vs stock prediction
│   └── crypto_forecast.ipynb
├── requirements.txt
└── README.md
```

Each folder contains:
- A clean notebook
- Commentary on methods used
- Visualizations
- Performance metrics (MSE, accuracy, F1, Sharpe, etc.)

---

## 📁 Modules Breakdown

### `classification_movement/direction_classifier_with_backtest.ipynb`
- Feature-rich XGBoost classifier
- Threshold tuning to optimize F1
- Final predictions used to simulate trading strategy
- Backtested vs buy-and-hold with Sharpe ratio and win rate

### `baseline_svr_xgboost/tesla_price_regression.ipynb`
- Compares SVR and XGBoost on TSLA close price
- Uses raw time index as input
- Establishes benchmark regression performance

### `technical_features/feature_engineered_model.ipynb`
- Adds SMA, EMA, RSI, % change, MACD, and lag features
- Improves predictive power of base model

### `deep_learning_lstm/lstm_price_forecast.ipynb`
- LSTM forecasting for multi-step stock price prediction
- Sequential modeling for temporal dynamics

### `crypto_modeling/crypto_forecast.ipynb`
- Repeats the pipeline on BTC or ETH
- Evaluates whether crypto behaves differently than stocks

### `backtesting_trades/strategy_backtest.ipynb`
- Modular notebook for strategy simulation based on model predictions
- Evaluates cumulative returns, Sharpe ratio, and win rate
- Can plug into multiple classifiers or forecasting outputs

---

## 📦 Installation

Run this to install dependencies:
```bash
pip install -r requirements.txt
```

Or run notebooks in **Google Colab** — pip cells included.

---

## 📈 Example Outputs
- 📊 Classification Accuracy: ~62%
- 💰 Strategy Return: +7.49%
- 📉 Buy & Hold Return: –14.39%
- 📈 Sharpe Ratio: 1.16
- 🧠 Model: XGBoostClassifier w/ class balancing, feature engineering, and threshold tuning

---

## 🚀 Future Work
- Add cross-validation / rolling windows
- Implement long/short strategies
- Expand to more stocks (AAPL, SPY, NVDA)
- Deploy as a Streamlit app

---

## 🙋‍♂️ Author
**Daivarsi Malik**  
Applied Modeling & Optimization  
This repo is part of a personal research initiative into quantitative trading and ML modeling.

---

## 📜 License
MIT License
