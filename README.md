# Jupyter Notebook Stock Analysis Script

This is a jupyter notebook for indepth stock analysis.

# Get Started

This jupyter notebook use yfiance library to pull stock's information

To install yfinance, type the following:
`conda install -c ranaroussi yfinance --yes`

Also, this script use mplfinance to render candle charts
To install mplfinace, type the following:
`pip install --upgrade mplfinance`

# Modify Your Stock Info.

In the third block, you can modify the stock number to the one you want to look at. In this example, we took '9988.hk' (BABA-SW). If you want to look at NASDAQ stocks, you can directly type the stock code (e.g. GME).

Also, you can select the period and the interval of the data. In this example, we set the period to 'max' and interval to '1d'.

````python
data = yf.Ticker('9988.HK')
df = data.history(period="max",interval="1d")
````



# Features

This Jupyter Notebook calcuate the average return of a given period. This Notebook calculate the Shape Ratio to dedue the risk and return.
