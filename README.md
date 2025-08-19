# Stock Market EDA & Risk Analysis  

## 📌 Project Description
This project performs **Exploratory Data Analysis (EDA)** on a selection of **US and Indian stocks** to study their **returns, volatility, risk and correlation**.  

The analysis lays the foundation for a future **AI-driven Stock Market Risk & Portfolio Optimizer** by quantifying risk, understanding diversification benefits, and highlighting market behavior under stress.  

---

## 📂 Data
- **Stocks Analyzed**  
  - US: `AAPL`, `MSFT`, `TSLA`  
  - India: `RELIANCE.NS`, `TCS.NS`, `HDFCBANK.NS`  
- **Data Source**: Yahoo Finance (`yfinance` library)  
- **Period**: Historical daily prices  

---

## 🔎 EDA Workflow
1. **Data Cleaning & Preparation**  
   - Download data using `yfinance`  
   - Handle missing values  
   - Convert closing prices to log returns  

2. **Statistical Analysis**  
   - Summary stats (Mean, Median, Std Dev)  
   - Distribution metrics (Skewness & Kurtosis)  
   - Percentiles (5th, 25th, 75th, 95th)  

3. **Volatility Analysis**  
   - Compare daily risk across US & Indian stocks  
   - Rolling volatility to track changes over time  

4. **Correlation Analysis**  
   - Stock-to-stock correlation matrices  
   - Internal group correlations (US vs India)    

5. **Visualizations**  
   - Cumulative returns with crash window  
   - Return distributions with skew/kurtosis  
   - Correlation heatmaps  
   - Pairplots of returns  

---



## 📈 Key Insights
- **Volatility**:  
  - US stocks (esp. TSLA) showed higher volatility than Indian stocks.  
  - Indian stocks are calmer day-to-day but still exhibit **fat tails**.  

- **Tail Risk (Kurtosis)**:  
  - JPM (not plotted in final set) showed very high kurtosis (extreme tail risk).  
  - Indian names (Reliance, HDFC, TCS) have fat-tailed distributions too.  

- **Correlation**:  
  - US group has higher internal correlation (~0.55).  
  - Indian group lower (~0.40).  
  - **Cross-market correlation is low** → combining US + Indian stocks improves diversification.  


---

## ⚙️ Tech Stack
- **Language**: Python 3  
- **Libraries**:  
  - `pandas`, `numpy` → data manipulation  
  - `matplotlib`, `seaborn` → visualization  
  - `yfinance` → stock market data  

---

## 🚀 How to Run
1. Clone the repo  
   ```bash
   git clone https://github.com/<your-username>/stock_market-eda.git
   cd stock-eda
