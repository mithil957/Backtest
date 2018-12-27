
*View on NBviewer - https://nbviewer.jupyter.org/github/mithil957/Backtest/blob/master/Market_Strats.ipynb

# Backtest
I wrote this notebook in order to backtest a stock trading idea I had. From the results, I didn't do that well compared to the Buy-and-hold strategy. However, I really enjoyed messing around with this code. There were a few times when I got insane returns like turning the intial $100 into 26 million in the course of 18 years. I am glad I ran into this because it helped me learn that I shouldn't always trust my results. I have turned the Jupyter Notebook into a html file so if you just want to check out the results then that is there for you. 

## The Strategy
Plot Bollinger Bands with standard deviation equal to .3 and moving average of 21 days. Then find the nearest peak(valley) point and if price is above(below) the Bollinger Bands and moves above(below) the nearest peak(valley) then go long(short). Exit the position if 2% has been gained or 1% has been lost (2:1 risk/reward ratio). This strategy boils to just buying a 'higher high' or selling a 'lower low' with Bollinger Bands as confirmation.

### Something to point out...
With this risk/reward ratio, the trader has to win at least win 33% of trades to be profitable. However, on the backtests preformed, some have win rates >33% but the returns are negative. This is because I used daily close data which means I would know the how much the market moved at the end, in other words the algo. would have a late reaction and could end up losing alot more than 2% or making more than 1%. This also means I can't exit positions as soon as risk/reward ratio has been satisfied. Quandl offers hourly data but I am only able to access the last 3 years which I don't think is good enough for a backtest.


Requirements: 
- In order to run the code, you will need to get an alpha vantage key and a quandl key.
- https://www.alphavantage.co/ and https://docs.quandl.com/

If you have any backtest ideas, shoot me an email at mviradia957@gmail.com. 
