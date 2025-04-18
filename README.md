<img src = "sc/1740065075355.jpg" alt = "img">

# Pairs Watch
Pairs Watch web app is a quantitative finance tool that helps users analyze potential pairs trading opportunities. <br/>

### Check out the app @ [streamlit.app](https://pairs-at-risk-f9sqcqqsmugxtlkpj2cvgr.streamlit.app/)
#

### Cointegration occurs when two or more non-stationary time series move together in the long run, forming a stationary linear combination.
<br/>

- Cointegration involves two steps: regressing one time series on the other to get the cointegration vector, and then perform an ADF test on the residuals of the regression to check for stationarity. <br/>

- If the residuals are not stationary, then we are estimating OLS beta (Sensitivity), not a long-term relationship. <br/>

- Therefore, residuals must be stationary.  <br/>

- The cointegration vector captures long term equilibrium relationship.  <br/>
#

#### Summary:
Regression to find the relationship (OLS assumes linear relationship, otherwise residuals will likely be non-stationary). <br/>
If the residuals are stationary, they fluctuate around a constant mean and do not drift indefinitely. Therefore, the pair is mean-reverting.

#

#### Strategy:
Calculating the percentiles of residuals is a great way to determine outliers that might indicate trading opportunities. <br/>
For example, if the residuals are far outside certain percentiles (e.g., the 5th or 95th percentile), that could signal that the price relationship is temporarily outside their usual bounds, creating a good chance for mean reversion (i.e., a return to the equilibrium).

<img src = "sc/resid_pairs.JPG" width = 1000 alt = "img">

<br/>

### [View Python code](https://github.com/s1dewalker/Cointegration/blob/main/py_files/Coint.ipynb)

