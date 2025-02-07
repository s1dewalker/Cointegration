## Cointegration for pairs trading | Nike and Adidas

Cointegration involves two steps: regressing one time series on the other to get the cointegration vector, and then perform an ADF test on the residuals of the regression to check for stationarity. <br/>

If the residuals are not stationary, then we are estimating OLS beta (Sensitivity), not a long-term relationship. <br/>

Therefore, residuals must be stationary.  <br/>

The cointegration vector captures long term equilibrium relationship.  <br/>

Calculating the percentiles of residuals is a great way to determine outliers that might indicate trading opportunities. <br/>
For example, if the residuals are far outside certain percentiles (e.g., the 5th or 95th percentile), that could signal that the price relationship is temporarily outside their usual bounds, creating a good chance for mean reversion (i.e., a return to the equilibrium).

#### [View Python code](https://github.com/s1dewalker/Cointegration/blob/main/py_files/Coint.ipynb)
