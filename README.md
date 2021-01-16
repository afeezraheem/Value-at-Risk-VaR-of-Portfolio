# Value-at-Risk-VaR-of-Portfolio

In this exercise, I used the Variance-Covariance Method to calculate the VaR of a portfolio of equities , relying on Yahoo! Finance historical stock prices API

Value at Risk,VaR, is a risk management technique to calculate the maximum loss an investment portfolio is likely to face in a specified time frame, given a certain degree of confidence. It is often used among a suite of financial metrics and models to help inform and shape investment and portfolio allocation decisions.

As in the attached Python code file, I calculated the following:

1. The periodic returns of the stocks in the select portfolio

2. The covariance matrix based on the returns calculated

3. The overall portfolio mean and standard deviation (weighted based on investment levels of each stock in portfolio)

4. Using the Norm object from scipy.stats, I calculated the inverse of the normal cumulative distribution with a specified probability, standard deviation, and mean

5. Finally, I estimated the VaR for the portfolio by subtracting the initial investment from the calculation in step 4

6. I calculated the VaR for expanded period windows, and studied the trend

Assumptions of VaR Portfolio Theory

5 underlying assumptions for VaR Portfolio concept are often identified in the literature. They include:

1. Stationarity: A 1-percentage fluctuation in returns is equally likely to occur at any point in time.

2. Random walk of intertemporal unpredictability: Day-to-day fluctuations in returns are assumed to be independent.

3. Nonnegativity: Financial assets with limited liability cannot attain negative values.

4. Time consistency. All single-period assumptions hold over the multiperiod time horizon.

5. Distributional. Daily return fluctuations follow a normal distribution with a mean of zero and a standard deviation of 100 basis points

In respect of these assumptions,the distributional assumption is often flawed. Stock returns, from historical perspective, have often been proven to not follow a normal distribution. However, using log normal distribution ( zero lower bounds, and long right tail) is more suitable. I intend to explore this approach in a future exercise

Added Tasks:

I installed yfinance, since fix_yahoo_finance had been decommissioned as Yahoo Finance historical market returns API


Refererence Materials:
https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.norm.html?fbclid=IwAR2gqmRetMwd-dH7lOYPpxITbYtqtuf25umX59FJh3J52byhJFWOSgG6xu4
https://financetrain.com/why-lognormal-distribution-is-used-to-describe-stock-prices/

