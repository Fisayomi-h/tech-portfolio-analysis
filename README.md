# tech-portfolio-analysis
Portfolio analysis of major tech stocks with performance, risk, and predictive metrics using Python.

Project Overview

This project analyzes the performance, risk exposure, and risk-adjusted returns of a technology-focused equity portfolio using historical market data.
The goal is to demonstrate how data analysis can support smarter investment, diversification, and rebalancing decisions.

The analysis is implemented entirely in Python (Jupyter Notebook) and focuses on real-world portfolio evaluation techniques used by investment firms, fintech companies, and asset managers.

 Problem Statement

As an investor holding multiple large-cap technology stocks:

How can we evaluate portfolio performance, risk exposure, and risk-adjusted returns over time in order to make informed allocation and rebalancing decisions?

Recruiters silently ask:

“Can this candidate help us make or protect money using data?”

This project answers that question using quantitative portfolio analytics.

 Objectives
Primary Objective

Evaluate the performance and risk characteristics of a technology equity portfolio using historical stock price data.

Specific Objectives

Measure individual stock performance

Assess portfolio-level returns using an equal-weighted strategy

Evaluate portfolio risk and downside exposure

Analyze risk-adjusted performance

Identify key drivers of portfolio risk

Support data-driven investment decisions

 Dataset Source

Historical adjusted close prices of U.S. large-cap technology stocks

Dataset stored locally as: Big_Tech_Dataset.xlsx

Structure includes:

date

stock_symbol

adj_close

 Selected Stocks

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

Cumulative Returns

Portfolio Daily Returns

Annualized Return

🔹 Risk Metrics

Annualized Volatility

Maximum Drawdown

Correlation Matrix

Rolling (20-day) Volatility

🔹 Risk-Adjusted Performance

Sharpe Ratio 

🔹 Portfolio Structure

Equal Weight Allocation

Risk Contribution (%) per stock

Identification of top risk drivers

🔹 Predictive / Forward-Looking Metrics

20-day Moving Average

50-day Moving Average

Rolling Volatility Trends

📈 Visualizations & Key Insights
1️⃣ Portfolio Growth

The portfolio shows long-term growth, but with significant drawdowns during market stress periods.

High-growth stocks drive returns, but also amplify volatility.

2️⃣ Risk & Drawdowns

Maximum drawdown highlights downside risk exposure.

Portfolio volatility confirms sensitivity to market shocks.

3️⃣ Diversification Insights

Correlation heatmap shows:

Strong correlations among some tech stocks

Partial diversification benefits, but not complete risk insulation

4️⃣ Risk Drivers

Risk contribution analysis reveals that:

A few stocks contribute disproportionately to portfolio risk

Portfolio risk is not evenly distributed despite equal weights

5️ Predictive Signals

Moving averages help identify:

Trend direction

Potential entry/exit or rebalancing signals

Rolling volatility shows changing risk regimes over time

 Key Results Summary
Metric	Result
Annualized Return	~29%
Annualized Volatility	~26%
Maximum Drawdown	~-49%
Sharpe Ratio	~0.96
Portfolio Nature	High return, high risk
 Conclusions & Recommendations
 Performance vs Risk

The portfolio delivers strong returns, but at the cost of high volatility.

Risk-adjusted performance (Sharpe Ratio < 1) suggests returns may not fully compensate for risk.

🔹 Concentration Risk

A small number of stocks drive most of the risk.

Equal weighting does not guarantee equal risk exposure.

🔹 Diversification Strategy

Consider adding:

Non-tech sectors

Defensive or low-correlation assets

This can improve drawdowns and risk-adjusted returns.

🔹 Rebalancing Insights

Rolling volatility and moving averages can inform:

Periodic rebalancing

Risk reduction during high-volatility periods

 Tools & Technologies

Python

Pandas & NumPy

Matplotlib & Seaborn

Jupyter Notebook

 Final Note

This project demonstrates how data analysis translates into investment insight, bridging the gap between raw market data and decision-making.

It is designed to reflect the type of analysis used in:

Asset Management

Fintech

Investment Research

Portfolio Analytics roles
