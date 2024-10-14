# Portfolio_Optimization_Basic
Portfolio Optimization Project This project implements a portfolio optimization algorithm using historical price data of selected financial assets. The optimization is based on the Markowitz Mean-Variance framework and uses the Sharpe Ratio as the objective function to maximize returns while minimizing risk.
It includes visualizations such as price trends, normalized prices, volatility clustering, and the Efficient Frontier to provide a comprehensive analysis of portfolio performance. 

Features Optimal Portfolio Weights: 
Calculates the optimal allocation of assets in the portfolio to maximize the Sharpe Ratio.
Price Trends: Visualizes the historical price trends of the selected assets.
Normalized Prices: Displays normalized prices to compare relative performance over time.
Volatility Clustering: Observes volatility patterns by plotting daily returns.
Efficient Frontier: Plots the efficient frontier to show the trade-off between portfolio risk and return. 
Python: The main programming language. 
Pandas: For data manipulation and analysis. 
NumPy: For numerical computations. Matplotlib: For plotting the visualizations. 
SciPy: Used for the optimization routines.
yfinance: For fetching historical stock data. 
FRED API: To retrieve the risk-free rate from the U.S. Treasury data. 

**PROJECT OVERVIEW**

**(1).** Data Collection Historical price data of assets is collected using yfinance. For this project, we use the following assets:  SPY (S&P 500 ETF) BND (Bond ETF) GLD (Gold ETF) QQQ (NASDAQ-100 ETF) VTI (Total Stock Market ETF) The data spans 5 years and includes adjusted close prices. 

**(2).** Portfolio Optimization The portfolio optimization is based on:  Expected Return: The annualized mean return of each asset. Portfolio Risk (Standard Deviation): Calculated using the covariance matrix of the log-normal returns. Sharpe Ratio: The portfolio is optimized to maximize the Sharpe Ratio, which is the ratio of excess return to risk.

**(3).** Risk-Free Rate The risk-free rate is fetched from the FRED API using the 10-year U.S. Treasury yield.  

**(4).** Constraints No short selling: Asset weights are bounded between 0 and 0.5 (maximum of 50% in a single asset). Weights must sum to 1 (fully invested portfolio). 

**(5).** Visualizations The following plots are included in the project:  Price Trends: The historical price trends for each asset. Normalized Prices: Shows the performance of each asset relative to a starting point (normalized to 1). Returns and Volatility Clustering: Plots daily returns to observe periods of volatility. Efficient Frontier: A curve showing the risk-return trade-off for different portfolio compositions. How to Run the Project Prerequisites Make sure you have the following libraries installed:  yfinance pandas numpy matplotlib scipy fredapi
