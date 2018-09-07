# Backtest
I wrote this notebook in order to backtest a stock trading idea I had. From the results, I didn't do that well compared to the Buy-and-hold strategy. However, I really enjoyed messing around with this code. There were a few times when I got insane returns like turning the intial $100 into 26 million in the course of 18 years. I am glad I ran into this because it helped me learn that I shouldn't always trust my results. I have turned the Jupyter Notebook into a html file so if you just want to check out the results then that is there for you. 

## The Strategy
Plot Bollinger Bands with standard devation equal to .3 and moving avegrage of 21 days. Then find the nearest peak(valley) point and if price is above(below) the Bollinger Bands and moves above(below) the nearest peak(valley) then go long(short). Exit the postion if 2% has been gained or 1% has been lost(2:1 risk/reward ratio). With this risk/reward ratio, the trader has to win atleast win 33% of trades to be profitable. This strategy boils to just buying a 'higher high' or selling a 'lower low' with Bollinger Bands as confirmation.   


Requirements: 
- In order to run the code, you will need to get an alpha vantage key and a quandl key.
- https://www.alphavantage.co/ and https://docs.quandl.com/

I am going to make updates to this, such as optimizing some of the parameters. Also, right now the backtest only takes into account 1 asset. I want to program it so it can backtest a given portfolio.

If you have any backtest ideas, shoot me an email at mviradia957@gmail.com. 
