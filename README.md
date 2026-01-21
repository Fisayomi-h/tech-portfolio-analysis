#  Tech-Portfolio-Analysis: From Risk-Heavy to Risk-Adjusted Growth

##  SITUATION
The Big Tech sector often provides high returns, but it is prone to extreme volatility and deep drawdowns. My initial analysis of an equal-weighted portfolio (**AAPL, AMZN, GOOGL, META, MSFT, NVDA, NFLX**) yielded a strong **29.21% annualized return** but was coupled with a dangerous **-49.09% Maximum Drawdown**. For most investors, a nearly 50% loss in capital is unacceptable, regardless of the upside.

##  TASK
My goal was to move from a **Descriptive** analysis (what happened) to a **Prescriptive** strategy (how to fix it). I aimed to:
1. ** Pinpoint specific assets contributing to disproportionate risk.
2. **Mathematically Optimize:** Rebalance weights to maximize the **Sharpe Ratio** using Monte Carlo simulations.
3. **Protect Capital:** Reduce the Maximum Drawdown to ensure capital preservation while maintaining competitive growth.

##  DATASET SOURCE
* **Source:** Historical adjusted close prices of U.S. large-cap technology stocks.
* **Storage:** Locally stored as `Big_Tech_Dataset.xlsx`.
* **Structure:** Includes `date`, `stock_symbol`, and `adj_close`.

##  SELECTED STOCKS
The portfolio focuses on 7 major technology leaders with diverse growth and volatility profiles:
**AAPL** (Apple), **AMZN** (Amazon), **GOOGL** (Alphabet), **META** (Meta Platforms), **MSFT** (Microsoft), **NVDA** (NVIDIA), **NFLX** (Netflix).

##  TOOLS & TECHNOLOGIES
1. **Python (Core Engine):** Data manipulation and matrix mathematics.
2. **Pandas & NumPy:** Financial time-series analysis and return calculations.
3. **Matplotlib & Seaborn:** Visualizing the Efficient Frontier and Stock Correlations.
4. **SciPy/Monte Carlo Simulation:** Running 2,000+ portfolio iterations to identify the optimal "Frontier."

##  ACTION
1. **Data Engineering:** Pivoted raw data into a time-series format and calculated daily percentage changes.
2. **Risk Assessment:** Conducted a correlation analysis to identify how these tech giants move in tandem.
3. **Trend Signal Development (Predictive):** Integrated 20-day and 50-day Moving Averages to identify Regime Shifts. I utilized these as predictive lead indicators to determine when momentum was exhausting and a defensive pivot was required.
4. **Efficient Frontier Simulation:** Developed a Monte Carlo simulation to generate 2,000 random weight combinations.
5. **Optimization:** Identified the **Maximum Sharpe Ratio** portfolio, the "North Star" where return-per-unit-of-risk is at its peak.

---

##  PERFORMANCE & RISK METRICS

### 🔹 Performance Visualization
1. **Daily Returns (Stock-level)**
<img width="1130" height="365" alt="Daily Returns Tech Portfolio Analysis" src="https://github.com/user-attachments/assets/417fb2e7-070c-41c4-8dc0-cda887ceef4c" />

2. **Cumulative Returns**
<img width="1130" height="433" alt="Cummulative returns" src="https://github.com/user-attachments/assets/00f30e93-d1c5-4d85-898e-5cf8087e8ea6" />

### 🔹 Risk & Correlation Matrix
**The Insight:** High positive correlations (near +1.0) mean these stocks often fall together. This explains the -49% drawdown; when the sector stumbled, there was nowhere to hide.
<img width="781" height="475" alt="Stock Correlation Matrix" src="https://github.com/user-attachments/assets/c6ce9b0f-f742-4981-91ca-3e97faba98ca" />

### 🔹 Momentum & Regime Shifts (Moving Averages)
**The Insight:** Looking at the 2022 period, the price dropped significantly below both the 20-day and 50-day averages. This indicates a **Regime Shift** from a bull to a bear market, proving that "Buy and Hold" was no longer the optimal strategy.
<img width="906" height="499" alt="Moving Averages" src="https://github.com/user-attachments/assets/47b20193-a023-4f52-a691-645249a80299" />

---

##  KEY INSIGHTS

### 1. What led to the 0.96 Sharpe Ratio?
* **The "Beta" Penalty:** The initial equal-weighted portfolio carried a high Beta (market sensitivity). Even with high gains, the quality of return was lower because the risk was uncompensated.
* **Uncompensated Volatility:** A Sharpe Ratio < 1.0 means we earned less than 1% of "excess return" for every 1% of risk taken. It suggests the portfolio was not perfectly diversified.
* **The Drawdown Impact:** The massive -49.09% drawdown increased the standard deviation (the denominator of the Sharpe formula), mathematically lowering the score.

### 2. Rolling Volatility Trends
* **Stable Leaders:** AAPL, MSFT, and GOOGL show relatively stable volatility.
* **Risk Drivers:** NFLX and NVDA are significantly more volatile, driving the majority of portfolio risk spikes.
* **Moderates:** META and AMZN show moderate volatility, offering slight diversification benefits.

### 3. The Efficiency Frontier Gap
The Equal Weight portfolio sat deep inside the Monte Carlo "cloud." This represents **uncompensated risk** the investor was taking on stress that wasn't producing additional profit. By moving to the **Frontier** (the top-left edge), we minimize risk for the highest possible return.

---

##  KEY RESULTS SUMMARY


| Metric | Equal-Weight (Initial) | Optimized (Final) | Business Impact |
| :--- | :--- | :--- | :--- |
| **Annualized Return** | 29.21% | 25.10% | Sustained High Growth |
| **Annualized Volatility** | 26.22% | **18.50%** | **~30% Risk Reduction** |
| **Sharpe Ratio** | 0.96 | **1.14** | **18.7% Efficiency Gain** |
| **Max Drawdown** | -49.09% | **-28.40%** | **42% Loss Protection (Saved 21% Portfolio Value)** |

**Optimized Asset Allocation (The Recipe):**
* **NVDA:** 45.09% | **NFLX:** 22.78% | **MSFT:** 10.44% | **META:** 0.27% (Divestment Target)

<img width="1001" height="528" alt="Portfolio Optimization" src="https://github.com/user-attachments/assets/e5dbe01e-c596-419a-a6bf-93a62d4c2060" />

---

##  RECOMMENDATIONS: STRATEGIC ACTION PLAN

1. **Immediate Rebalancing to Risk-Parity Weights:** Move away from equal dollar amounts. I recommend trimming high-beta stocks (NVDA) and increasing weights in lower-volatility anchors like **MSFT** or **AAPL** to protect against the 49% drawdown risk.
2. **Adopt Tactical Trend Following:** Utilize the 20/50-day Moving Average crossovers. When a "Death Cross" occurs, the portfolio should rotate into cash or defensive ETFs to preserve capital.
3. **Dynamic Exit for Low-Efficiency Assets:** Based on the 0.27% allocation recommendation for **META**, I recommend divesting from assets where the volatility does not justify the return, freeing up liquidity for higher-conviction drivers.
4. **Diversification Beyond Tech:** To achieve a **Sharpe Ratio > 1.5**, the next phase must introduce non-correlated assets (e.g., Value stocks or Commodities) to further flatten the -28% drawdown curve.

---

##  CONCLUSION
This project proves that **Data Analysis + Economic Logic** is the best defense for capital. By sacrificing a small amount of raw return, I was able to significantly improve risk-adjusted performance and capital preservation, moving from a reactive strategy to a **prescriptive investment workflow.**
