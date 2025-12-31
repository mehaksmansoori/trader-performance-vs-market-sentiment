# Trader Performance vs Market Sentiment

#Note - “Submitted as part of Primetrade.ai Internshala assignment – Mehak Shaikh Mansoori”

## 📌 Overview
This project analyzes the relationship between **Bitcoin market sentiment** (Fear & Greed Index) and **trader performance** using historical trading data from **Hyperliquid**.  
The goal is to uncover sentiment-driven patterns and translate them into **actionable trading strategy insights**.


## 📊 Datasets Used

### 1. Bitcoin Fear & Greed Index
- **Columns:** Date, Value, Classification (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)
- Represents overall market sentiment on a daily basis.

### 2. Hyperliquid Historical Trader Data
- **Columns include:**  
  Account, Symbol, Execution Price, Size USD, Side, Timestamp, Closed PnL, Leverage, etc.
- Contains real historical trade-level data.


## 🧠 Methodology

1. Loaded and cleaned both datasets
2. Converted timestamps and aligned data on a daily level
3. Merged trader data with sentiment data using date
4. Analyzed:
   - Average PnL per sentiment
   - Total PnL per sentiment
   - Trade activity across sentiments
5. Derived **strategy recommendations** based on relative profitability


## 📈 Key Insights

- **Fear and Neutral** market conditions show **above-average profitability**
- **Greed and Extreme Greed** exhibit lower risk-adjusted returns
- Traders tend to perform better using **contrarian strategies**
- Extreme bullish sentiment increases volatility and downside risk


## 🧩 Strategy Recommendations

- **Fear / Neutral:** Favorable for aggressive trading with controlled risk
- **Greed:** Moderate opportunity; trade selectively
- **Extreme Greed:** Reduce exposure and prioritize risk management


## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook


## ▶️ How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Open the notebook: jupyter notebook trader_performance_vs_market_sentiment.ipynb
