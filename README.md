# AutomatedTradingSystem
This Python GUI stock trading simulator uses simple threshold strategies to suggest buy/sell actions by comparing the current price with recent lows and highs (over 3, 5, and 10 intervals). It visualizes data, tracks portfolio and transactions, helping users "buy low, sell high" based on short-term price trends.
## Features

- Fetches intraday stock data (5-minute intervals) using `yfinance`
- Displays stock price data and suggested trading actions
- Visualizes stock price trends with matplotlib charts
- Tracks a virtual portfolio with owned stocks and quantities
- Records transaction history for buys and sells
- Multiple simple strategies to suggest buy/sell decisions based on recent lows and highs
- User-friendly interface built with Tkinter
- Disclaimer: This app is for educational purposes only; all trades are simulated.

## Trading Strategies

The app uses three short-term strategies comparing the current stock price with the minimum and maximum prices over recent intervals (3, 5, and 10 data points) to suggest:

- **Buy Now:** If current price is at or below recent minimum
- **Sell Now:** If current price is at or above recent maximum
- **Hold:** Otherwise

The final suggestion is based on the majority vote of these strategies.

## Installation

1. Install required libraries:
   ```bash
   pip install yfinance matplotlib pandas pytz
