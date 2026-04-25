# XJTLU_ACC102_Individual-Assignment_Ruoxi.Zhang
Stock risk-return analysis for ACC102 individual assignment
# Stock Analysis Tool

A Python-based stock analysis tool that connects to the WRDS (Wharton Research Data Services) database to perform comprehensive stock performance analysis and visualization.

## Features

- **Multi-Stock Comparison**: Analyze and compare multiple stocks simultaneously
- **Two Analysis Modes**:
  - **Mode A**: Compare stocks across different industries
  - **Mode B**: Compare stocks within the same industry
- **Comprehensive Visualizations**:
  - Stock Price Trend Chart
  - Cumulative Returns Plot
  - Risk vs Return Scatter Plot
  - 30-Day Rolling Volatility Chart
  - Correlation Heatmap
  - Efficient Frontier Analysis with randomized portfolio weights
- **Performance Metrics**:
  - Sharpe Ratio calculation and ranking
  - Portfolio optimization visualization

## Prerequisites

- Python 3.x
- WRDS account credentials
- Required Python packages:
  - `wrds`
  - `pandas`
  - `numpy`
  - `matplotlib`

## Installation

```bash
pip install wrds pandas numpy matplotlib
```

## Usage

1. Run the Jupyter notebook `Untitled.ipynb`
2. Enter your WRDS username and password when prompted
3. Select analysis mode (A or B)
4. Enter stock tickers (comma-separated, e.g., `AAPL,TSLA,JPM,KO`)
5. Enter the start date for analysis (format: `YYYY-MM-DD`)
6. View the generated charts and performance metrics
7. Optionally try another date or exit

## Data Source

All stock price data is retrieved from the CRSP (Center for Research in Security Prices) database via WRDS.

## Example

```
Select Mode:
A = Compare different industries
B = Compare stocks in same industry
Enter A or B: A
Enter stock tickers (comma separated, e.g. AAPL,TSLA,JPM,KO): AAPL,TSLA,JPM,KO
Enter start date (YYYY-MM-DD): 2022-01-01
```

## Output

The tool generates the following outputs:
1. **Price Trend** - Raw stock price movements over time
2. **Cumulative Returns** - Cumulative return performance
3. **Risk vs Return** - Scatter plot comparing volatility and average returns
4. **Rolling Volatility** - 30-day rolling standard deviation
5. **Correlation Heatmap** - Pairwise correlation between stocks
6. **Sharpe Ratio Ranking** - Risk-adjusted return ranking
7. **Efficient Frontier** - Portfolio optimization visualization

## Technical Details

- Uses CRSP daily stock file (`crsp.dsf`) for price data
- Handles missing data through forward-fill and dropna methods
- Generates 3,000 random portfolio combinations for efficient frontier analysis
- Includes auto-reconnection logic for WRDS database connection issues

## Note

Ensure your WRDS account has access to the CRSP database before running the analysis.
