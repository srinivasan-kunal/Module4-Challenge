# Analyzing portfolio risk and returns

This challenge requires the evaluation of 4 investment options in terms of their risk and returns to assess the the suitability of their inclusion in the client's portfolios.

---

## Technologies

Key python libraries required for the program have been imported in the first code block and includes- `pandas`, `numpy', `pathlib` and `%matplot inline`  


---

## Installation Guide

In case pandas or numpy modules are unavailable the following commands in the terminal will help install them.

```python
pip install pandas

pip install numpy
```
---

## Usage

Python function `cumprod()` on the returns data from the four options and the S&P 500 shows BERKSHIRE Fund had the highest returns over the period, followed by TIGER Fund while the other two had negative returns. It may also be noted that all the four options have a return rate significantly less than the returns on S&P 500 over the period of analysis. The plot of the cumulated returns reveals that in the initial period until early 2016 the three of four investment options provided a return higher than S&P 500, primarily due to a significant drop in the returns on S&P500. 

Analysis of the variance using the pandas `describe()` function and the pandas `plot.box` shows that of the four options- TIGER Fund had the least volatility in returns while BERKSHIRE Fund had the most. The same is confirmed by the annualized standard deviation calculation done with function support from pandas and numpy.

A 3 week rolling standard deviation plot using pandas `rolling(window=)` helps assess the volatility trend smoothened out for noise. The historical trends point out a change in volatility pattern in BERKSHIRE Fund & PAULSON Fund. 

Pandas functions `mean()` and `std()` allow us to calculate the annualized sharpe ratios for the four fund options over the period and notifies of positive sharpe ratios for BERKSHIRE Fund & TIGER Fund.

Further deepdive into the two Funds with positive sharpe ratios, using pandas `cov()` and `std()` function allows us to review the trend in the funds' beta values overtime. Based on 2 month rolling beta values it was concluded that although volatile, BERKSHIRE Fund has had the highest return over the analysis period while TIGER Fund has shown modest returns with lower volatility.

It was concluded that a portfolio strategy for maximum returns may consider maximizing investments in BERKSHIRE Fund while a more conservative strategy may include TIGER Fund in the mix to provide some stability in returns. 

---

## Contributors


Kunal Srinivasan

---

## License

2022 edX Bootcamps 