NVDA Stock Price Analysis
A Python project analyzing NVIDIA (NVDA) stock price trends using moving averages and rolling volatility.

What it does
Pulls historical NVDA price data via the yfinance API
Computes 20-day and 50-day moving averages to identify trend signals
Calculates rolling 20-day annualized volatility
Generates a summary report and a chart visualizing price trend + volatility
Exports the full processed dataset to CSV
Why I built this
I wanted hands-on practice applying the same data analysis workflow I used in my Diabetes Risk Prediction project (cleaning data, feature engineering, drawing conclusions from a dataset) to a financial/markets context. Moving averages and volatility are basic but foundational tools in equity research and technical analysis, and this was a way to build that intuition directly in code rather than just reading about it.

How it works
python nvda_analysis.py
The script:

Fetches 1 year of NVDA daily price data
Computes short-term (20-day) and long-term (50-day) moving averages
Flags a bullish/bearish trend signal based on which moving average is higher
Computes annualized rolling volatility from daily returns
Saves a chart (nvda_analysis.png) and a CSV export of the full dataset
Example output
==================================================
NVDA Price Analysis Summary
==================================================
Period: 2025-06-30 to 2026-06-30
Latest Close: $XXX.XX
20-day MA: $XXX.XX
50-day MA: $XXX.XX
Trend signal: bullish/bearish
Total return over period: XX.XX%
Average annualized volatility: XX.XX%
==================================================
Tech used
Python
pandas / numpy for data processing
yfinance for live market data
matplotlib for visualization
