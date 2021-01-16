# Value-at-Risk-VaR-of-Portfolio

In this exercise, I used the Variance-Covariance Method to calculate the VaR of a portfolio of equities , relying on Yahoo! Finance historical stock prices API

Value at Risk,VaR, is a risk management technique to calculate the maximum loss an investment portfolio is likely to face in a specified time frame, given a certain degree of confidence. It is an often calculated metric used within a suite of financial metrics and models to help inform and shape investment decisions.

As in the attached Python code file, I calculated the following:

1. The periodic returns of the stocks in your portfolio

2. The covariance matrix based on the returns calculated

3. The overall portfolio mean and standard deviation (weighted based on investment levels of each stock in portfolio)

4. Using the Norm object from scipy.stats, I calculated the inverse of the normal cumulative distribution with a specified probability, standard deviation, and mean

5. Finally, I estimate the VaR for the portfolio by subtracting the initial investment from the calculation in step 4

6. I calculated the VaR for expanded period windows, and studied the trend



