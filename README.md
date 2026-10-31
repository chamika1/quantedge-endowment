# Quant Edge 1.0 - Final Challenge

Team n0T4ounD - Sabaragamuwa University of Sri Lanka

Portfolio and risk analysis for the Serendib University Endowment Fund
(USD 10,000,000, conservative mandate).

## Run the app

```
pip install -r requirements.txt
streamlit run app.py
```

## What is in here

- `app.py` - the Streamlit app (portfolio, risk dashboard, backtesting,
  stress testing, assumptions and limitations)
- `quantedge/` - the calculations: portfolio construction, VaR / ES / EVT,
  backtesting (Kupiec, Christoffersen, Basel), stress tests
- `data/` - cleaned price data (Yahoo Finance, 2007-2026) and the FRED
  risk-free rate
- `scripts/` - `download_data.py` gets the data, `run_analysis.py` runs
  the full analysis
- `results/` - the output tables of the analysis

## Recommended portfolio

SPY 13.3%, EFA 5.5%, EEM 5.0%, AGG 40.0%, GLD 20.0%, XLE 11.2%, XLK 5.0%

A minimum-variance portfolio with policy constraints (every asset between
5% and 40%, at least 25% in bonds, at most 60% in equities, at most 20% in
gold). Details, risk numbers and the reasoning are in the report and in
the app.
