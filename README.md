# BIST Retail Stocks: Return and Risk Analysis

How do BIMAS, MGROS and SOKM compare in terms of historical returns and investment risk against the BIST 100 index? I wanted to examine whether retail stocks show defensive characteristics and how their risk and performance change over time.

Data and Tools

* Stocks: BIMAS.IS, MGROS.IS, SOKM.IS
* Benchmark: XU100.IS (BIST 100)
* Period: 3 years of historical daily data
* Data source: Yahoo Finance
* Tools: Python, Pandas, NumPy, Matplotlib, SQLite and SQL

Findings

1. Annualized returns: BIMAS had the highest annualized return at 35.38%, followed by MGROS at 4.72%. SOKM recorded a negative return of -12.23%, while the BIST 100 returned 10.35%. BIMAS outperformed the benchmark, whereas MGROS and SOKM underperformed it.
2. Volatility and beta: SOKM had the highest annualized volatility (36.93%), followed by BIMAS (36.05%) and MGROS (34.50%). All three stocks had beta values below 1 (BIMAS: 0.93, MGROS: 0.83, SOKM: 0.90), although their total volatility was higher than the BIST 100 (24.56%).
3. Maximum drawdown: SOKM experienced the largest maximum drawdown (-54.34%), followed by MGROS (-44.05%) and BIMAS (-33.47%). This shows that lower beta does not necessarily mean lower downside risk.
4. April–August 2025: The 60-day rolling volatility chart shows a noticeable increase in volatility across the retail stocks during this period. BIMAS and SOKM reached approximately 50%, while MGROS peaked around 42%, compared with approximately 32% for the BIST 100. This does not support the idea that these stocks consistently behave as defensive investments.

Methodology

* Daily returns are calculated using percentage changes in adjusted closing prices.
* Annualized returns are calculated using the compound annual growth rate (CAGR).
* Annualized volatility is calculated using the standard deviation of daily returns multiplied by the square root of 252 trading days.
* Beta is estimated using the covariance between each stock’s daily returns and the BIST 100 returns, divided by the benchmark variance.
* Maximum drawdown is calculated by comparing prices with their historical running maximum.
* Rolling volatility is calculated over a 60-day window.
* SQL is used to query the best and worst daily returns for each stock.

Limitations

* Historical performance does not guarantee future results.
* Transaction costs, taxes and inflation are not included.
* The analysis focuses on historical price data and does not consider fundamental financial indicators or company-specific news.

Data retrieved on 27 November 2026 from a single source.
