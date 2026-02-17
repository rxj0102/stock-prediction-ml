# 📈 Stock Price Prediction with Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)

A comprehensive machine learning project for predicting stock prices using various algorithms and feature engineering techniques. This project demonstrates an end-to-end ML pipeline from data collection to trading strategy implementation, with a focus on quantitative finance applications.

## 🎯 Project Highlights

- **64 engineered features** including technical indicators (RSI, MACD, Bollinger Bands)
- **22+ models tested** across multiple algorithm families
- **Walk-forward validation** for time series integrity
- **Trading strategy backtesting** with comprehensive metrics
- **Production-ready code** with modular design

## 📊 Results on AAPL (2018-2024)

| Metric | Best Model | Value |
|--------|------------|-------|
| RMSE | Linear Regression | 2.43 |
| R² | Linear Regression | 0.984 |
| MAPE | Linear Regression | 1.13% |
| Direction Accuracy | Gradient Boosting | 80.5% |
| Strategy Return | ML-based | +75.7% |
| Buy & Hold Return | Benchmark | +28.7% |
| Sharpe Ratio | ML Strategy | 3.42 |


🧪 Models Implemented

Linear Models

✅ Linear Regression
✅ Ridge Regression (L2 regularization)
✅ Lasso Regression (L1 regularization)
✅ ElasticNet
Tree-based Models

✅ Random Forest
✅ XGBoost
✅ LightGBM
✅ Gradient Boosting
Ensemble Methods

✅ Voting Regressor
✅ Stacking Regressor
✅ Weighted Average Ensemble
Neural Networks

✅ MLP Regressor
✅ Custom architectures
📈 Feature Engineering

Price-based Features

Returns and log returns
Price ranges and typical prices
Lag features (1,2,3,5,10 days)
Technical Indicators

RSI (Relative Strength Index)
MACD (Moving Average Convergence Divergence)
Bollinger Bands
Volume indicators
Advanced Features

Price momentum
Volume-price correlation
Support/resistance levels
Market regime indicators
📊 Evaluation Metrics

RMSE - Root Mean Square Error
MAE - Mean Absolute Error
R² - R-squared score
MAPE - Mean Absolute Percentage Error
Direction Accuracy - Percentage of correct direction predictions
Sharpe Ratio - Risk-adjusted returns
💼 Trading Strategy

The project includes a simple trading strategy based on model predictions:

Buy when predicted price > current price + threshold
Sell when predicted price < current price - threshold
Hold otherwise
Strategy performance vs Buy & Hold:

Strategy Return: +75.7%
Buy & Hold: +28.7%
Outperformance: +163%
Sharpe Ratio: 3.42

## 🚀 Quick Start

### Prerequisites
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/stock-prediction-ml.git
cd stock-prediction-ml

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
pip install -e .  # Install package in development mode
