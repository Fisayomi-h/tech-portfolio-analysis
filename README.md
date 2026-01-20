# Tech-Portfolio-Analysis


Tech Portfolio Optimization: From Risk-Heavy to Risk-Adjusted Growth

  SITUATION

The "Big Tech" sector often provides high returns, but it is prone to extreme volatility and deep drawdowns. My initial analysis of an equal-weighted portfolio (AAPL, AMZN, GOOGL, META, MSFT, NVDA, NFLX) yielded a strong 29.21% annualized return but was coupled with a dangerous -49.09% Maximum Drawdown. For most investors, a nearly 50% loss in capital is unacceptable, regardless of the upside.

 TASK

My goal was to move from a Descriptive analysis (what happened) to a Prescriptive strategy (how to fix it). I aimed to:

    Identify the specific assets contributing to disproportionate risk.

    Mathematically optimize the portfolio weights to maximize the Sharpe Ratio.

    Reduce the Maximum Drawdown to protect capital while maintaining competitive growth.

    
 DATASET SOURCE

Historical adjusted close prices of U.S. large-cap technology stocks

Dataset stored locally as: Big_Tech_Dataset.xlsx


Structure includes:

date

stock_symbol

adj_close


 SELECTED STOCKS

To maintain clarity and realism, the portfolio focuses on 7 major technology leaders:

AAPL (Apple)

AMZN (Amazon)

GOOGL (Alphabet)

META (Meta Platforms)

MSFT (Microsoft)

NVDA (NVIDIA)

NFLX (Netflix)

These stocks represent different growth, volatility, and correlation profiles within the tech sector.

 KPIs & Metrics Analyzed


 TOOLS & TECHNOLOGIES

    Python (Core Engine): Used for data manipulation and matrix mathematics.

    Pandas & NumPy: For financial time-series analysis and return calculations.

    Matplotlib & Seaborn: For visualizing the Efficient Frontier and Stock Correlations.

    SciPy/Monte Carlo Simulation: To run 2,000+ portfolio iterations to identify the optimal "recipe."


 ACTION

    Data Cleaning: Pivoted raw transactional data into a time-series format and calculated daily percentage changes.

    Risk Assessment: Conducted a correlation analysis to identify how these tech giants move in tandem.

    Efficient Frontier Simulation: Developed a Monte Carlo simulation to generate 2,000 random weight combinations, calculating the Return, Volatility, and Sharpe Ratio for each.

    Optimization: Identified the "Maximum Sharpe Ratio" portfolio—the specific point on the frontier where the return-per-unit-of-risk is at its peak.

    
🔹 Performance Metrics

Daily Returns (stock-level)
<img width="1130" height="365" alt="Daily Returns Tech Portfolio Analysis" src="https://github.com/user-attachments/assets/417fb2e7-070c-41c4-8dc0-cda887ceef4c" />

Cumulative Returns
<img width="1130" height="433" alt="Cummulative returns" src="https://github.com/user-attachments/assets/00f30e93-d1c5-4d85-898e-5cf8087e8ea6" />

Portfolio Daily Returns

Annualized Return


🔹 Risk Metrics

Annualized Volatility

Maximum Drawdown

Correlation Matrix

What it shows: A heatmap of how closely each stock's price moves in relation to the others (scaled from -1 to +1).

The Insight: High positive correlations (near +1.0) across the Big Tech sector mean that these stocks often fall at the same time. This explains the -49% drawdown; when one giant stumbled, they all did.

<img width="781" height="475" alt="Stock Correlation Matrix" src="https://github.com/user-attachments/assets/c6ce9b0f-f742-4981-91ca-3e97faba98ca" />

Rolling (20-day) Volatility


🔹 Risk-Adjusted Performance

Sharpe Ratio 


🔹 Portfolio Structure

Equal Weight Allocation

Risk Contribution (%) per stock

Identification of top risk drivers


🔹 Predictive / Forward-Looking Metrics

What it shows: The average price of an asset over the last 20 trading days, smoothing out daily "noise."

The Insight: When the actual price falls below the 20-day MA, it indicates a loss of short-term momentum.
20-day Moving Average
<img width="906" height="499" alt="Moving Averages" src="https://github.com/user-attachments/assets/47b20193-a023-4f52-a691-645249a80299" />

50-day Moving Average

Rolling Volatility Trends
<img width="904" height="497" alt="Screenshot 2026-01-15 102624" src="https://github.com/user-attachments/assets/b006a4a3-b70f-48f6-bc55-7ca4aafc79b8" />

<img width="904" height="497" alt="Screenshot 2026-01-15 102713" src="https://github.com/user-attachments/assets/e47d5f5d-1776-4125-ac1e-c77ea56fd277" />

<img width="903" height="500" alt="Screenshot 2026-01-15 102757" src="https://github.com/user-attachments/assets/d74ebd35-c720-432a-b481-104f34d58b5b" />

📈 Visualizations & Key Insights

 PORTFOLIO GROWTH

The portfolio shows long-term growth, but with significant drawdowns during market stress periods.

High-growth stocks drive returns, but also amplify volatility.


 RISK & DRAWDOWNS

Maximum drawdown highlights downside risk exposure.

Portfolio volatility confirms sensitivity to market shocks.


 DIVERSIFICATION INSIGHTS

Correlation heatmap shows:

Strong correlations among some tech stocks

Partial diversification benefits, but not complete risk insulation


 RISK DRIVERS

Risk contribution analysis reveals that:

A few stocks contribute disproportionately to portfolio risk

Portfolio risk is not evenly distributed despite equal weights


 PREDICTIVE SIGNALS

Moving averages help identify:

Trend direction

Potential entry/exit or rebalancing signals

Rolling volatility shows changing risk regimes over time


 KEY RESULTS SUMMARY
METRIC	RESULT

Annualized Return	~29%
Annualized Volatility	~26%
Maximum Drawdown	~-49%
Sharpe Ratio	~0.96
Portfolio Nature	High return, high risk

By shifting from an Equal-Weight strategy to a Mathematically Optimized strategy, I achieved the following:

Metric,              Equal-Weight (Initial),  Optimized (Final),        Impact
Annualized Return,     29.21%,                   25.10%,            Sustained High Growth
Annualized Volatility, 26.22%,                   18.50%,           ~30% Risk Reduction
Sharpe Ratio,          0.96,                     1.14,18.7%         Efficiency Gain
Max Drawdown,          -49.09%,                  -28.40%,           Saved ~21% of Portfolio Value
<img width="963" height="339" alt="Screenshot 2026-01-20 162911" src="https://github.com/user-attachments/assets/c159a2ec-8748-4bab-ae11-255ac7ee06bb" />

 INSIGHTS: What the Data Revealed
 
 Performance vs Risk
The portfolio delivers strong returns, but at the cost of high volatility.

Risk-adjusted performance (Sharpe Ratio < 1) suggests returns may not fully compensate for risk.

 The NVDA Risk-Reward Paradox: While NVDA was the primary engine of growth (contributing heavily to the 29.21% return), it was also the primary driver of volatility. In a team-based portfolio context, its raw performance was "punished" by the optimizer to protect the overall floor of the investment.

 The Inefficiency of Equal Weighting: My analysis proved that an equal-weight approach (20% per stock) ignores the "risk-contribution" of individual assets. While simple to implement, this strategy resulted in a -49.09% drawdown, indicating that the portfolio was unintentionally over-exposed to the most volatile assets.

 Diversification Drivers vs. Dead Weight: The simulation identified NFLX (22.78%) and MSFT (10.44%) as high-efficiency diversifiers. Conversely, META (0.27%) was identified as "dead weight," where the risk of holding the stock did not justify its expected return compared to other available tech assets.

The Efficiency Frontier Gap: The "Equal Weight" portfolio sat deep inside the Monte Carlo cloud, rather than on the edge. This gap represents uncompensated risk, meaning the investor was taking on stress that wasn't producing additional profit.
<img width="905" height="552" alt="Screenshot 2026-01-20 162957" src="https://github.com/user-attachments/assets/833ba83a-01e4-4f3c-b810-e8ad0f8f48d5" />

<img width="1001" height="528" alt="Portfolio Optimization" src="https://github.com/user-attachments/assets/e5dbe01e-c596-419a-a6bf-93a62d4c2060" />

 RECOMMENDATIONS: Strategic Action Plan
 

Immediate Rebalancing to Maximum Sharpe Weights: I recommend a tactical shift from equal weights to the Optimized Recipe (NVDA 45%, NFLX 22%, MSFT 10%). This re-weighting is projected to improve the Sharpe Ratio by 18.7%, providing a superior risk-adjusted return profile.

Implement a Risk-Parity Framework: Stop allocating capital based on dollar amounts and start allocating based on volatility contribution. High-beta stocks like NVDA should be capped during high-volatility regimes to prevent the -49% drawdown observed in Phase 1.

Adopt Tactical Trend Following: Utilize the 20-day and 50-day Moving Average crossover strategy on core holdings like AAPL. When the short-term average falls below the long-term average (a "Death Cross"), the portfolio should rotate into cash or defensive ETFs to preserve capital.

Dynamic Exit for Low-Efficiency Assets: Based on the 0.27% allocation recommendation for META, I recommend a complete divestment from underperforming high-volatility assets to free up liquidity for higher-conviction, more efficient growth drivers like MSFT or GOOGL.

Cross-Sector Hedging: To break the high correlation within the "Big Tech" cluster, the next phase of this strategy should include 0% to 15% allocation in non-correlated sectors (e.g., Treasury bonds or defensive Consumer Staples) to further flatten the volatility curve.


Portfolio Analytics roles
