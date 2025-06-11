# 📈 Stock Price EDA: Microsoft, Apple, Google, NVIDIA
## 📌 Objective
This project explores and compares historical stock price trends of four major tech companies — Microsoft (MSFT), Apple (AAPL), Google (GOOGL), and NVIDIA (NVDA). The goal is to identify patterns, compare performance, and uncover business insights based on time series data.
## 🛠️ Tools & Libraries
* Python
* [yfinance](https://pypi.org/project/yfinance/) for downloading stock data
* pandas for data wrangling
* matplotlib & seaborn for data visualization
* Jupyter Notebook
## 📊 Techniques
* Time series data loading and preprocessing
* Calculation of Daily Log Returns and Cumulative Log Returns
* Kernel Density Estimation (KDE) for daily log return distribution analysis
* 7-Day Rolling Volatility Calculation and Visualization
* Correlation Matrix Analysis for Daily Log Returns/Profits
* Comparative trend visualization across multiple stocks (Closing Prices, Cumulative Returns)
## 🔍 Key Insights
* **Overall Performance & Trends (2022-2024):**
    * All four stocks demonstrated a long-term upward trend in closing prices, though with varying fluctuations.
    * NVIDIA showed the most significant absolute price increase and high volatility in its price trajectory.
    * Microsoft consistently held the highest absolute closing price and exhibited a smoother, more stable growth curve.
    * Apple and Google also displayed smoother growth curves compared to NVIDIA, but at lower absolute price levels than Microsoft.

* **Cumulative Log Returns (May-Aug 2024):**
    * **NVIDIA** exhibited the highest cumulative growth performance (peaking at ~1.65x initial value) alongside significant fluctuations, indicating high potential returns with high risk.
    * **Apple** achieved the second-highest cumulative growth (~1.4x initial value) with a relatively smooth and steady trend, reflecting consistency and a lower risk profile compared to NVIDIA.
    * **Microsoft** showed stable, positive cumulative growth, but at a more modest rate (~1.05x initial value), characterized by a very smooth curve.
    * **Google** had the least consistent cumulative performance, at times falling below its initial starting level (ratio < 1), highlighting a risk in maintaining positive long-term growth.

* **Daily Log Return Distribution (May-Aug 2022):**
    * **NVIDIA** had the highest daily volatility, indicated by the widest and lowest Kernel Density Estimation (KDE) curve with extended tails, suggesting frequent large price swings.
    * **Microsoft** was the most stable, with the tallest and narrowest KDE curve, signifying tightly clustered daily returns around zero and minimal volatility.
    * **Apple** showed low daily volatility but with a slightly wider positive tail than Google, implying potential for significant upside days despite overall stability.
    * **Google** exhibited average daily volatility with a notable bias towards negative returns (longer negative tail), consistent with slower accumulation.

* **7-Day Rolling Volatility (May-Aug 2024):**
    * **NVIDIA** consistently maintained the highest rolling volatility (often > 3%, peaking > 7%), underscoring its high short-term risk.
    * **Microsoft** had the lowest and most stable rolling volatility (mostly < 1.5%, rarely exceeding 2%), confirming its low-risk profile.
    * **Apple** showed moderate to high rolling volatility, with occasional spikes exceeding 3%.
    * **Google** displayed moderate rolling volatility, generally between 1% and 2.5%, though sometimes dipping below 1%.
    * Notably, Microsoft, Apple, and Google all experienced periods where their 7-day rolling volatility dropped below 1%.

* **Correlation of Daily Log Returns (May-Aug 2024):**
    * All pairwise correlations between the stocks were positive, indicating a tendency to move in the same direction.
    * **Google and Microsoft** exhibited the strongest correlation (~0.70), suggesting highly synchronized daily movements.
    * **NVIDIA** showed the lowest correlation with other stocks (ranging from 0.28 to 0.45). This implies NVIDIA could offer some portfolio diversification, helping to reduce overall portfolio volatility and mitigate downside risk when combined with the other stocks.
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
│ └── kde_daily_log_returns_may_aug_2024.png
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