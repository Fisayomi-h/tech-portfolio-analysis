# Tech-Portfolio-Analysis
Portfolio analysis of major tech stocks with performance, risk, and predictive metrics using Python.


  PROJECT OVERVIEW
  
This project analyzes the performance, risk exposure, and risk-adjusted returns of a technology-focused equity portfolio using historical market data.
The goal is to demonstrate how data analysis can support smarter investment, diversification, and rebalancing decisions.

The analysis is implemented entirely in Python (Jupyter Notebook) and focuses on real-world portfolio evaluation techniques used by investment firms, fintech companies, and asset managers.


 PROBLEM STATEMENT
 
As an investor holding multiple large-cap technology stocks:

How can we evaluate portfolio performance, risk exposure, and risk-adjusted returns over time in order to make informed allocation and rebalancing decisions?


 OBJECTIVES
 
Primary Objective
Evaluate the performance and risk characteristics of a technology equity portfolio using historical stock price data.

Specific Objectives
Measure individual stock performance

Assess portfolio-level returns using an equal-weighted strategy

Evaluate portfolio risk and downside exposure

Analyze risk-adjusted performance

Identify key drivers of portfolio risk

Support data-driven investment decisions


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
<img width="781" height="475" alt="Stock Correlation Matrix" src="https://github.com/user-attachments/assets/c6ce9b0f-f742-4981-91ca-3e97faba98ca" />

Rolling (20-day) Volatility


🔹 Risk-Adjusted Performance

Sharpe Ratio 


🔹 Portfolio Structure

Equal Weight Allocation

Risk Contribution (%) per stock

Identification of top risk drivers


🔹 Predictive / Forward-Looking Metrics

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

 CONCLUSIONS & RECOMMENDATIONS
 
 Performance vs Risk
The portfolio delivers strong returns, but at the cost of high volatility.

Risk-adjusted performance (Sharpe Ratio < 1) suggests returns may not fully compensate for risk.

 Concentration Risk
A small number of stocks drive most of the risk.

Equal weighting does not guarantee equal risk exposure.

 DIVERSIFICATION STRATEGY

Consider adding:

Non-tech sectors

Defensive or low-correlation assets

This can improve drawdowns and risk-adjusted returns.


 REBALANCING INSIGHTS

Rolling volatility and moving averages can inform:

Periodic rebalancing

Risk reduction during high-volatility periods


 TOOLS & TCHNOLOGIES
 
Python

Pandas & NumPy

Matplotlib & Seaborn

Jupyter Notebook


 FINAL NOTE

This project demonstrates how data analysis translates into investment insight, bridging the gap between raw market data and decision-making.

It is designed to reflect the type of analysis used in:

Asset Management

Fintech

Investment Research

Portfolio Analytics roles
