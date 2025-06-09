# Stock EDA Analysis
This project performs Exploratory Data Analysis (EDA) on stock prices of four major companies: MSFT, AAPL, GOOGL, and NVDA.

Data is fetched directly from Yahoo Finance using the `yfinance` library.  
All analysis and visualization are done in the notebook `notebooks/stock_eda.ipynb`.

---

## Project Structure
```plaintext
stock-eda-analysis/
│
├── notebooks/
│ └── stock_eda.ipynb # Notebook for data collection and analysis
├── reports/ # Folder to save generated plots and images
├── requirements.txt # Required Python libraries
└── README.md

## Install dependencies
pip install -r requirements.txt

## How to run
Open the notebook notebooks/stock_eda.ipynb using Jupyter Notebook or Jupyter Lab.

Run cells sequentially to download data, perform analysis, and generate plots.

Generated plots are saved in the reports/ folder.

Main libraries used:
yfinance
numpy
pandas
matplotlib
seaborn

## Project goals
Collect 2 years of historical stock price data for MSFT, AAPL, GOOGL, and NVDA (01-01-2022 to 31-12-2024).

Perform descriptive statistics and volatility analysis.

Visualize price trends and trading volumes.

Compare performance and risk between stocks.
