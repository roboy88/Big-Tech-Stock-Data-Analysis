# Big-Tech-Stock-Data-Analysis
# Big Tech Stock Data Analysis 📈🤖

## TL;DR (in human language)
This project uses Python to look at historical stock prices for big technology companies and answer questions like:
- Which stock grew more over time?
- Which stock is “wigglier” (more risky)?
- Do some stocks move together like besties?

We turn raw price data into charts and simple risk metrics so you can *see* patterns instead of guessing.

> ⚠️ Not financial advice. This is a data project, not a “get rich quick” spell.

---

## What’s in this repo
- `BIG_Tech_Stock_Data_analysis.ipynb` — the main analysis notebook
- `AIStocktrackerapp.ipynb` — an additional notebook (app/experiment)
- `README.md` — this file

---

## Big idea (the “why”)
Stocks go up and down because humans are… humans.  
Instead of vibes, this project uses data to measure:

### 1) Growth
If a stock’s price increases over time, it grew.

### 2) Daily Returns
A **return** is the gain or loss over time, often written as a percent. (Example: +2% in a day.)  
Returns help compare days fairly, even when prices are very different.  
_Source: Investopedia definition of “return.”_  [oai_citation:1‡Investopedia](https://www.investopedia.com/terms/r/return.asp?utm_source=chatgpt.com)

### 3) Trend (Moving Average)
A **moving average** is like a “smoother” line that averages the last N days so the chart is less noisy.  
_Source: Investopedia moving average explanation._  [oai_citation:2‡Investopedia](https://www.investopedia.com/terms/m/movingaverage.asp?utm_source=chatgpt.com)

### 4) Risk (Volatility)
**Volatility** means how much returns bounce around. More bounce = more risk.  
_Source: Investopedia volatility definition._  [oai_citation:3‡Investopedia](https://www.investopedia.com/terms/v/volatility.asp?utm_source=chatgpt.com)

### 5) Risk-Adjusted Performance (Sharpe Ratio)
The **Sharpe ratio** compares reward vs. risk: higher usually means “better return for the risk taken.”  
_Source: Investopedia Sharpe ratio overview._  [oai_citation:4‡Investopedia](https://www.investopedia.com/terms/s/sharperatio.asp?utm_source=chatgpt.com)

---

## Visualizations you’ll see (and what they mean)
1. **Normalized Price Chart**  
   Everyone starts at the same starting point (like 100) so you can compare growth fairly.

2. **Daily Returns Chart / Histogram**  
   Shows how often the stock has small days vs. huge jumps.

3. **Rolling Volatility**  
   A “risk over time” chart. It answers: *When was this stock extra chaotic?*

4. **Correlation Heatmap**  
   Shows which stocks tend to move together.  
   +1 = move together, 0 = unrelated, -1 = opposite directions.

---

## How to run it (local)
1. Install Python 3.10+.
2. Install packages:
   ```bash
   pip install pandas numpy matplotlib yfinance