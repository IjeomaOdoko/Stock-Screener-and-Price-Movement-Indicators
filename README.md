# Stock-Screener-and-Price-Movement-Indicators

This purpose of this project was to create a stock screener based on market cap, download the pricing data, and create different price movement charts. 

The following python libraries were utilized to achieve this: 

- *[pandas_datareader](https://pandas-datareader.readthedocs.io/en/latest/)* to import historical data on stocks.

- *[pandas](https://pandas.pydata.org/)* for working with large data sets.

- *[datetime](https://docs.python.org/3/library/datetime.html)* for handling date and time datatypes.

- *[matplotlib](https://matplotlib.org/)* for data visualization.

- *[get-all-tickers](https://pypi.org/project/get-all-tickers/)* to get lists of stocks from NYSE, NASDAQ, and AMEX. .

- *[mplfinance](https://github.com/matplotlib/mplfinance)* to create price movement charts.

- *[ipwidgets](https://ipywidgets.readthedocs.io/en/latest/) to provide interactivity within the jupyter notebook.


## Price Movement Charts 

Price movement charts help with timing the market for buying or selling opportunities by determining up and down trends in price movement. These charts can typically be used with any financial time series like stocks, bonds, options, futures or commodities. 

[Example codes and charts created in python here](https://github.com/IjeomaOdoko/Stock-Screener-and-Price-Movement-Indicators/tree/master/Code). 

### Renko 
Is a type of price movement chart that has no time dimension. The key parameter it requires is the box size which signifies each brick (price movement size). The box size can be set to a specific value, or it be set to be equal to the ATR (average true range) which is derived from the closing price of the stock. With these charts its able to quickly tell the direction of trend changes.

### PNF
PNF otherwise known as Point and Figure Chart is very similar to the renko chart, in that it also does not have a time dimension. An X represents when the price has moved higher, and an O represents when the price has dropped. The PNF also has a box size that can be set as a specific value, or be equal to the ATR (average true range).

### OHLC

This is a type of price movement chart that captures the open, high, low and closing prices for each given trading day.

The vertical line represents the range in prices from high to low for the day. The horizontal lines extending out from the vertical line, represents open price for the left, and close price for the right. 
![OHLC indicator.png](https://github.com/IjeomaOdoko/Stock-Screener-and-Price-Movement-Indicators/blob/master/pictures/OHLC%20price%20Indicator%20.png)
### Candlestick 

Also known as Japanese candlesticks are a type of price movement chart that takes into consideration both price, time and volume. It helps to determine the sentiment of the market - Bullish or Bearish. Bullish - would indicate a buy, while Bearish - would indicate short or sell for a stock trader.

Candlestick patterns can help determine price direction and momentum. One key thing to note when using candlesticks to understand price movement, it is important to first identify the market trend, before finding candlestick patterns in the data. Candlestick patterns are also best suited for identifying short term price movements.

#### Long vs Short Days 

Long days refers to large price movement within the trading day, and short days refers to low price movement within the trading day. This comparison however is best suited for short-term price movement of about 5-10days. 

![Candlestick Lines.png](https://github.com/IjeomaOdoko/Stock-Screener-and-Price-Movement-Indicators/blob/master/pictures/Candlestick%20indicator%20.png)

## References: 

Morris, Gregory L., 1948-, Candlestick charting explained timeless techniques for trading stocks and futures [electronic resource], New York : McGraw-Hill, c2006, 3rd ed.

[Price Movement Charts](https://github.com/matplotlib/mplfinance/blob/master/examples/price-movement_plots.ipynb)

[Renko Charts](https://www.investopedia.com/terms/r/renkochart.asp)

[PNF Charts](https://www.investopedia.com/terms/p/pointandfigurechart.asp)










