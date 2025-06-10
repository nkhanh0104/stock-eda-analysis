# 📈 Stock Price EDA: Microsoft, Apple, Google, NVIDIA
## 📌 Objective
This project explores and compares historical stock price trends of four major tech companies — Microsoft (MSFT), Apple (AAPL), Google (GOOGL), and NVIDIA (NVDA). The goal is to identify patterns, compare performance, and uncover business insights based on time series data.
## 🛠️ Tools & Libraries
- Python
- [yfinance](https://pypi.org/project/yfinance/) for downloading stock data
- pandas for data wrangling
- matplotlib & seaborn for data visualization
- Jupyter Notebook
## 📊 Techniques
- Time series data loading and preprocessing
- Rolling average calculation to smooth out short-term volatility
- Comparative trend visualization across multiple stocks
## 🔍 Key Insights
- **NVIDIA** shows the highest price volatility among the four stocks in recent months.
- **Apple** and **Microsoft** exhibit more stable and consistent growth.
- Rolling average effectively reveals long-term upward/downward trends and helps filter out daily price noise.
- All four stocks generally follow similar macro trends, with differences in magnitude and recovery speed.
## 📁 Project Structure
```plaintext
stock-eda-analysis/
│
├── data/
│ └── AAPL_Close_2022_2025.csv # AAPL Close Price from 2022 to 2025
│ └── GOOGL_Close_2022_2025.csv # AAPL Close Price from 2022 to 2025
│ └── MSFT_Close_2022_2025.csv # AAPL Close Price from 2022 to 2025
│ └── NVDA_Close_2022_2025.csv # AAPL Close Price from 2022 to 2025
├── notebooks/
│ └── stock_eda.ipynb # Notebook for data collection and analysis
├── reports/ # Folder to save generated plots and images
│ └── closing_prices_2022_2024.png
│ └── correlation_heatmap_may_aug_2024.png
│ └── cumulative_log_returns_may_aug_2024.png
│ └── daily_log_returns_may_aug_2024.png
│ └── kde_daily_returns_may_aug_2024.png
│ └── rolling_volatility_may_aug_2024.png
│ └── volatility_bar_chart_may_aug_2024.png
├── requirements.txt # Required Python libraries
└── README.md```
## 📘 How to Run
1. Clone this repository:
  ```bash
  git clone https://github.com/nkhanh0104/stock-eda-analysis.git
  cd stock-eda-analysis```
  
2. (Optional) Create and activate a virtual environment
- python -m -venv venv
- source venv/bin/activate # or venv\Scripts\activate on Windows

3. Install required libraries
- pip install -r requirements.txt

4. Launch Jupyter Notebook:
- jupyter notebook

5. Open stock_eda_analysis.ipynb and run the cells

✍️ Author
Nguyen Nhu Khanh
Aspiring Data Scientist with strong software development background, currently exploring time series data analysis in finance.