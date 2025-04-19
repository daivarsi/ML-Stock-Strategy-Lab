# 📊 Stock Modeling Lab

An evolving, modular project exploring machine learning and deep learning techniques for forecasting stock price trends, volatility, and movement. Using real market data and powerful models, each module investigates a different question in quantitative finance and time-series prediction.

---

## 🔍 Objective
**Can modern ML models capture financial price behavior better than traditional methods?**

From SVR to LSTMs, from technical indicators to trade simulation — this lab demonstrates practical, progressive solutions for stock prediction.

---

## 🧱 Repository Structure

```
stock-modeling-lab/
├── baseline_svr_xgboost/            # 🔹 Baseline regression using SVR + XGBoost
├── technical_features/             # 🔹 Add moving averages, RSI, volume, etc.
├── classification_movement/        # 🔹 Predict direction (up/down) instead of price
├── deep_learning_lstm/             # 🔹 LSTM for time-series forecasting
├── backtesting_trades/             # 🔹 Simulate trades based on model predictions
├── crypto_modeling/                # 🔹 Compare crypto vs stock prediction
├── requirements.txt
└── README.md
```

Each folder contains:
- A clean notebook
- Commentary on methods used
- Visualizations
- Performance metrics (MSE, accuracy, etc.)

---

## 📁 Modules Breakdown

### `baseline_svr_xgboost/`
- Compares SVR and XGBoost on Tesla stock
- Uses only time index as input
- Evaluates fit using MSE and R²

### `technical_features/`
- Adds indicators like SMA, EMA, RSI
- Tests whether additional signals improve prediction
- Uses feature engineering + XGBoost

### `classification_movement/`
- Reframes the problem: up/down instead of price
- Binary classifier using logistic regression, XGBoost
- Evaluates using accuracy, precision, recall, F1

### `deep_learning_lstm/`
- Builds a sequential LSTM model with Keras
- Uses time windows as input sequences
- Evaluates forecasting ability for 1–5 day predictions

### `backtesting_trades/`
- Simulates trading decisions based on predicted signals
- Tracks portfolio returns vs buy-and-hold strategy
- Incorporates win rate, drawdown, cumulative profit

### `crypto_modeling/`
- Applies models to BTC-USD or ETH-USD
- Compares performance against traditional stocks
- Analyzes differences in trend behavior and volatility

---

## 🛠 Getting Started

Install dependencies:
```bash
pip install -r requirements.txt
```

Or run each notebook in **Google Colab** with necessary pip cells included.

---

## 📈 Example Visuals
- Model predictions vs actual
- Confusion matrix (classification)
- Trade profit curves
- Feature importance plots

---

## 🧠 Future Ideas
- LSTM + Attention
- Hybrid models (technical + news sentiment)
- Cross-stock generalization testing

---

## 🙋‍♂️ Author
**Daivarsi Malik**  
Applied Modeling & Optimization  
Feel free to fork, run experiments, or suggest new modules.

---

## 📜 License
MIT License

