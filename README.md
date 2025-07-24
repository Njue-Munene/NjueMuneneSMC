
# NjueMuneneSMC

## 📈 Smart Money Concepts (SMC) Pattern Detection with RSI Divergence

This project implements an automated system to detect **W and M patterns** in forex charts using **Smart Money Concepts (SMC)**, combined with **Relative Strength Index (RSI) divergence**. The strategy is designed to identify high-probability swing trade setups on the 1-hour timeframe for major currency pairs like EURUSD.

---

## 🚀 Features

- 🔍 Detects **W/M reversal patterns** algorithmically
- 📊 Confirms entries using **RSI divergence**
- ✅ Validates trades with **Break of Structure (BoS)** before **Change of Character (ChoCH)**
- 🧠 Implements key SMC principles (liquidity grabs, internal structure, mitigations)
- 📉 Backtesting included with key performance metrics:
  - Win rate
  - Risk-Reward ratio
  - Total PnL
  - Profit factor
- 📁 Exports trade logs and signal data to CSV

---

## 📂 Project Structure

```
NjueMuneneSMC/
├── NjueMuneneSMC.ipynb     # Main Jupyter Notebook (core logic + backtest)
├── signals_*.csv           # Auto-generated signal logs (per symbol)
├── trade_results.csv       # Final backtest results
├── README.md               # Project documentation
```

---

## ⚙️ How It Works

1. **Data Ingestion**  
   Reads OHLCV data for selected forex pairs.

2. **Pattern Detection**  
   Scans for W/M structures using peak-trough logic and custom rules.

3. **RSI Divergence**  
   Confirms whether RSI forms higher lows (for W) or lower highs (for M) to validate momentum shifts.

4. **Smart Money Confirmation**  
   Applies BoS/ChoCH logic before marking a trade as valid.

5. **Backtesting**  
   Simulates trades using configurable RR and stop loss rules.

---

## 📈 Example Output

```
Total Signals:           101
Completed Trades:        92
Wins:                    53
Losses:                  39
Win Rate:                57.6%
Avg Risk-Reward:         1.95
Avg PnL per Trade:       +13.9
Total PnL (USD):         +1407.5
```

---

## 🛠️ Requirements

- Python 3.10+
- Pandas
- NumPy
- Matplotlib
- TA-Lib or `ta` library
- Jupyter Notebook

Install dependencies:

```bash
pip install pandas numpy matplotlib ta
```

---

## 🧠 Strategy Summary

This system is built on real-world price action and smart money behavior. The main idea is to:

- Identify manipulation zones
- Confirm buyer/seller intent via RSI
- Enter trades post-BoS when structure shifts in our favor

---

## 📌 Future Improvements

- Add multi-timeframe analysis
- Integrate with MT5 or TradingView for live alerts
- Deploy as a Streamlit dashboard for non-coders
- Refine pattern recognition with deep learning (optional)

---

## Risk Disclaimer

This trading strategy is for educational purposes only. Past performance does not guarantee future results. Always conduct thorough testing and risk management before live trading.

---

## 👤 Author

**Njue Munene**  
Quant Developer | AI Engineer | Web Developer  
🔗 [LinkedIn](https://www.linkedin.com/in/njue-munene-)

---


