# XJTLU_ACC102_Individual-Assignment_Ruoxi.Zhang
Stock risk-return analysis for ACC102 individual assignment
# Stock Risk & Return Analysis with WRDS

This project is a Python-based financial analysis tool that connects to the WRDS (Wharton Research Data Services) database, retrieves stock price data, and visualizes the relationship between risk (standard deviation of returns) and return (mean return) for selected stocks.

## Features

- Connect to WRDS securely using the `wrds` Python library.
- Choose between:
  - **Mode A**: Compare stocks from different industries.
  - **Mode B**: Compare stocks within the same industry.
- Input custom stock tickers and a start date.
- Fetch historical price data from the CRSP database.
- Clean and process data to calculate daily returns.
- Generate a scatter plot of **Risk vs. Return** for the selected stocks.
- Loop to test different start dates without restarting the notebook.
- Automatically handle connection errors and reconnect to WRDS if needed.

## Requirements

- Python 3.7+
- WRDS account (with access to CRSP)
- PostgreSQL `.pgpass` file setup (automatically created by the script)

## Python Libraries

- `wrds`
- `pandas`
- `numpy`
- `matplotlib`
- `psycopg2-binary`
- `sqlalchemy`

You can install dependencies using:

```bash
pip install wrds pandas matplotlib
