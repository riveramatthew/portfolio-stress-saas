# Portfolio Stress Testing and Scenario Analysis

This project provides a Python tool to perform stress testing and scenario analysis on investment portfolios. It fetches historical stock data, simulates economic scenarios (e.g., market crash, interest rate hike), and calculates potential impacts on portfolio value. It also includes a basic Value at Risk (VaR) calculation using historical simulation.

## Features
- Fetch historical stock data using Polygon API.
- Define custom portfolios with tickers and weights.
- Simulate scenarios like market crashes or sector-specific shocks.
- Calculate portfolio returns, volatility, and VaR.
- Visualize results with charts.

## Requirements
- Python 3.8+
- Libraries: `polygon-api-client`, `pandas`, `numpy`, `matplotlib`

Install via:

pip install -r requirements.txt

## Usage
1. Get a free API key from [polygon.io](https://polygon.io) and set it as an environment variable: `export POLYGON_API_KEY=your_key_here`.
2. Open `stress_test.ipynb` in Jupyter Notebook or JupyterLab.
3. Run the cells to fetch data, define your portfolio, and run simulations.
4. Customize scenarios in the notebook.

Example Portfolio:
- AAPL: 40%
- GOOGL: 30%
- TSLA: 30%

Scenarios:
- Market Crash: -30% on all stocks.
- Tech Bubble Burst: -50% on tech stocks.

## Data Source
Historical data from Polygon API (daily closes for the past year).

## Limitations
- Requires internet for data fetching.
- Simplistic models; not for production use without enhancements.
- Assumes no transaction costs or dividends.

## Contributing
Fork the repo and submit pull requests for improvements, e.g., adding Monte Carlo simulations or more factors.

## License
MIT License
