# Macro–Market Data Analysis

A Python workflow for aligning macroeconomic series with financial-market data and examining how cross-asset relationships change over time.

## Purpose

This project connects economic indicators and market prices in a single analytical workflow. It is designed to support questions such as how monetary conditions relate to equity risk, how inflation-linked variables interact with defensive assets, and how real-economy signals connect with commodity-sensitive securities.

The asset universe, analytical window and report outputs are intentionally configuration-dependent while the broader reporting framework is being standardized.

## Analytical Scope

- Retrieval of macroeconomic series from Federal Reserve Economic Data (FRED)
- Retrieval of market prices through Yahoo Finance
- Frequency alignment and resampling across macro and market datasets
- Rolling-correlation analysis
- Rolling annualized-volatility analysis
- Correlation heatmaps and synchronized time-series visualizations
- Automated generation of a research-oriented PDF output

## Workflow

1. Download economic and market series.
2. Clean and align observations with different reporting frequencies.
3. Build a consolidated analytical dataset.
4. Calculate returns, rolling correlations and volatility measures.
5. Produce visual diagnostics and a concise analytical report.

## Repository Contents

| File | Description |
|---|---|
| [macro_financial_analytics.py](./macro_financial_analytics.py) | Data retrieval, transformation, analysis and visualization workflow |
| [Macro_Impact_Analysis_Report.pdf](./Macro_Impact_Analysis_Report.pdf) | Example analytical output generated from the workflow |

## Tools and Data Sources

- Python: Pandas, NumPy, Matplotlib and Seaborn
- Data access: pandas-datareader and yfinance
- Sources: FRED and Yahoo Finance

## Interpretation

The analysis is descriptive and diagnostic. Correlations may vary across samples and market regimes, and they should not be interpreted as causal relationships. Results also depend on data availability, frequency alignment and the selected lookback window.

## Development Context

This repository documents a focused macro–market research module. Related cross-asset monitoring and macro-risk work is presented in [Macro Outlook & Markets Analysis](https://github.com/caballerohh/Macro-Outlook-and-Markets-Analysis).

---

This project is provided for research, education and professional portfolio purposes. It does not constitute investment advice.
