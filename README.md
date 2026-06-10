# Pairs Trading Strategy — Indian Stock Market

A Python project that identifies cointegrated stock pairs from NSE and builds 
a statistical arbitrage trading strategy using Z-score mean reversion.

## What it does
- Downloads historical data for 17 NSE stocks (2021-2024)
- Builds a correlation heatmap to identify related stocks
- Tests cointegration between HDFC Bank and Kotak Bank
- Runs ADF test to check stationarity of spread and ratio
- Calculates Z-score to identify entry and exit points
- Generates buy and sell signals using rolling Z-score (5 day / 20 day MA)

## Trading Pair
HDFC Bank (HDFCBANK.NS) and Kotak Bank (KOTAKBANK.NS)
— both private sector banks, highly correlated, same sector

## Universe of stocks screened
Reliance · TCS · Infosys · HDFC Bank · ICICI Bank · SBI · L&T ·
Bharti Airtel · ITC · HUL · Kotak Bank · Axis Bank · Maruti ·
Asian Paints · Sun Pharma · Bajaj Finance · Nestle

## Key parameters
- Data Range: 2021-01-01 to 2024-01-01
- Z-score Buy Signal: below -1.0
- Z-score Sell Signal: above +1.0
- Short MA window: 5 days
- Long MA window: 20 days

## Libraries used
yfinance · pandas · numpy · matplotlib · seaborn · statsmodels

## Installation
pip install yfinance pandas numpy matplotlib seaborn statsmodels

## How to run
Open the notebook in Jupyter and run all cells top to bottom.

## Environment
Python 3.11 · Jupyter Notebook · ChromeOS Linux
