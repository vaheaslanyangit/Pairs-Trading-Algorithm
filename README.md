# Pairs Trading Algorithm - README.md

## Introduction
This Pairs Trading Algorithm is a financial trading strategy that leverages statistical and quantitative analysis to trade pairs of highly correlated assets. It seeks to identify and exploit the divergence in the prices of these assets. This README provides detailed instructions on setting up and running the algorithm.

## Requirements
- Python 3.x
- Libraries: numpy, pandas, matplotlib, yfinance, ib_insync (for interactive brokers integration)
- Data Source: Yahoo Finance (via yfinance library)

## Installation
Use pip to install the required libraries:
```bash
pip install numpy pandas matplotlib statsmodels yfinance ib_insync
```


## Usage
1. **Import Libraries:** Import necessary Python libraries including numpy, pandas, matplotlib, and yfinance.
2. **Define Ticker Symbols:** Set the ticker symbols for the asset pairs you want to trade (e.g., KO and PEP).
3. **Data Retrieval:** Fetch historical prices for the tickers from Yahoo Finance.
4. **Data Processing:**
   - Calculate the rolling mean and standard deviation for each asset.
   - Compute the z-scores for each asset.
   - Determine the spread between the two assets.
   - Calculate the rolling mean and standard deviation of the spread.
5. **Signal Generation:**
   - Generate long and short signals based on the spread.
   - Determine the positions for each asset.
   - Implement a long-only strategy (optional).
6. **Performance Calculation:**
   - Compute the percentage change and portfolio returns.
   - Calculate total logarithmic returns and plot the results.
7. **Trading Signal Visualization:** Plot various aspects of the trading strategy for analysis.

## Example Plots
- Spread between assets
- Trading signals for each asset
- Cumulative returns comparison with buy-and-hold strategy

## Additional Features
- The algorithm includes an example with simulated data using an AR(1) model.
- Visualization of rolling statistics and trading signals.
- Comparison of cumulative returns with and without position holding.

## Disclaimer
This algorithm is provided for educational purposes only. It does not constitute financial advice. Users should conduct their own due diligence before trading.

