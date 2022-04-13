# finance_analysis
3 file: arima_model, basic_analysis, yf_scrapping

# arima_model:

Use to predict the stock price

# basic_analysis:

using yfinance library to get certain stock price chart, volatility, market cap, with MA50 and MA200 for longterm investing. 

Display the above information for basic understanding of the stock price

#yf_scrapping:

srap yahoo finance website for that company's financial statement then print out for further analysis

#price_model:

Currently coding: 

1/ Using yfinance library to display the opening price with interval of 1d from 2015 until current date 

2/ Dividing the stock opening price into smaller "batches group by year"

	- Ex: batch1 is from '2022-01-01' to current date; batch2 is from '2021-01-01' to '2022-01-01',...

3/ Using various methods for trading to compare which method is the best by simulating the trading methods.

	- Method currently using: 
		
		- Displaying SMA21,50 for current batch's basic trend lines as:
			if SMA21 > SMA50 gives a potential buy (long) signal
			else gives a sell (short) signal

		- Also displaying EMA20 against the Opening price chart for current batch's Opening price:
			if EMA20 is above the price gives a potential buy (long) signal 
			else gives a potential sell (short) signal
	_ Other methods to consider: applying RSI, MACD, etc  for more correct buy/sell signals

Potential project to do:
	- Predict/Analyze stock price by scrapping news from Twitter to identify the hot news of certain stocks or stocks trending on that day
	- For certain stock analysis, after scrapping the news, identify if they are bad or good news to produce a more indept understanding of the price movement 