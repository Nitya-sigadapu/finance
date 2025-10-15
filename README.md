# finance
# 📈 Mean Reversion Trading Strategy – Indian Equities

### 🎯 Objective
To design and backtest algorithmic trading strategies based on **mean reversion principles** within **Indian equity markets**, exploring statistical signals and regime-based behaviour.

---

## 🧠 Core Concept
Mean reversion assumes that asset prices tend to revert back to their statistical mean after deviation. The strategy identifies **overbought/oversold zones** and executes trades expecting price reversal.

---

## 🔍 Strategy Variations Explored

| Variant | Indicator Used | Logic |
|--------|--------------|------|
| **Z-Score Reversion** | Z = (Price - SMA) / Std Dev | Enter long when Z < -threshold and short when Z > threshold |
| **Bollinger Band Reversion** | SMA ± k * Std Dev | Buy near lower band expecting price pullback to mean |
| **RSI-Based Reversion** | RSI 0–100 range | Buy when RSI < 30 (oversold), sell when RSI > 70 (overbought) |

---

## ⚙️ Technical Implementation

- **Data Source:** Indian Equities (NSE Stocks)
- **Mean Definitions:** `Simple Moving Average (SMA)`, `Exponential Moving Average (EMA)`
- **Volatility Filtering:** Trade only when rolling standard deviation exceeds calibrated threshold
- **Regime Detection:** Strategy evaluated separately under **bull**, **bear**, and **sideways** markets
- **Tools Used:** `Python`, `Pandas`, `NumPy`, `Matplotlib`, `Streamlit (optional UI version)`

---

## 📊 Backtesting Metrics Considered

| Metric | Description |
|--------|------------|
| **Hit Ratio** | Percentage of profitable trades |
| **Max Drawdown** | Risk assessment under adverse market moves |
| **Sharpe / Sortino Ratio** | Risk-adjusted return |
| **Average Holding Period** | Measures strategy aggressiveness |
| **Equity Curve Plot** | Visual representation of P&L growth |

---

## 🚀 Future Enhancements

- Add **position sizing using Kelly Criterion**
- Integrate **transaction cost modeling for Indian market liquidity**
- Deploy as **Streamlit dashboard** with adjustable parameters
- Compare performance with **Buy-and-Hold Benchmark (NIFTY50)**

---

## 📌 Project Relevance

✔️ Good **entry-level quant strategy**  
✔️ Demonstrates **signal generation → backtest → evaluation pipeline**  
✔️ Shows understanding of **market regimes & statistical filters**  
✔️ Strong addition to **Quant/Trading Internship Resume**
