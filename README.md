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
