Quantitative Trading & Technical Analysis with Python
This repository contains a collection of Python notebooks designed for stock market analysis, technical indicator visualization, and algorithmic trading strategy backtesting. Leveraging financial data from Yahoo Finance (yfinance), these tools allow traders and analysts to visualize market trends and test hypothesis-driven strategies.

📂 Repository Contents
1. Technical Indicators.ipynb
A comprehensive tool for calculating and visualizing key technical indicators used in financial market analysis.

Functionality: Fetches historical stock data and overlays multiple technical indicators on price charts.

Indicators Calculated:

SMA & EMA: Simple and Exponential Moving Averages for trend identification.

MACD: Moving Average Convergence Divergence (including Signal Line) for momentum tracking.

RSI: Relative Strength Index to identify overbought/oversold conditions.

Bollinger Bands: Upper, Middle, and Lower bands to measure volatility.

Visualization: Generates dual-axis subplots to display price action alongside indicator values.

2. Ema&RSI combine.ipynb
An algorithmic trading backtesting engine that implements a hybrid trend-following and mean-reversion strategy.

Strategy Logic:

Entry Signal (Trend): Buys (Long) when Price > EMA; Sells (Short) when Price < EMA.

Exit Signal (Momentum): Exits Long positions when RSI indicates Overbought (>70); Exits Short positions when RSI indicates Oversold (<30).

Backtesting Engine:

Simulates trades based on generated signals (defaulting to 100 shares per trade).

Calculates daily portfolio value including cash and stock holdings.

Computes compounded daily returns.

Performance Metrics & Plots:

Equity Curve: Tracks total portfolio value over time.

Drawdown: Visualizes peak-to-trough decline to assess risk.

Volatility: Plots rolling standard deviation of returns.

🛠️ Technologies Used
Python 3.x

yfinance: For fetching historical market data.

Pandas & NumPy: For data manipulation, vectorized calculations, and window functions.

Matplotlib: For rendering financial charts and equity curves.
