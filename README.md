# Markowitz-mean-variance-portfolio-optimizer

Using the efficient frontier theory and the Sharpe ratio, we find the portfolio with the maximum risk-adjusted return.

We start by downloading price data for five different assets: S&P 500 (SPY), QQQ, TLT, Gold (GLD), and Bitcoin (BTC-USD).  
Then we calculate the monthly returns for each asset, as well as the average return vector and covariance matrix.

We define the portfolio performance (expected return, volatility, and Sharpe ratio) and set the constraints for the optimization (long-only, weights sum to 1).  
The optimization is done by minimizing the negative Sharpe ratio, which is equivalent to maximizing the Sharpe ratio.

Once the optimal weights are obtained, we calculate the annualized portfolio return, volatility, and Sharpe ratio.  
Finally, we plot the Efficient Frontier using 10,000 randomly generated portfolios and mark the optimal portfolio on the plot with a red star.

### Output
- Annualized return  
- Annualized volatility  
- Sharpe ratio  
- Optimal portfolio weights  
- Efficient Frontier plot with the optimal portfolio highlighted

### Libraries used
`numpy`, `scipy`, `matplotlib`, `yfinance`

