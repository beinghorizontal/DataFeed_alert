# DataFeed_alert
Play alert when local data feed is interrupted. 

It is for charting and execution tool called MultiCharts which uses its own Power Language which is a fork of TradeStation's Easy Language.

This work is based on the article https://www.tradingcode.net/multicharts/alerts/data-feed-alert/

The code in the article is for real-time data feed from broker API to MultiCharts but it doesn't work for local data feed such as Universal DDE. Since my use case is mostly getting data from Python to Multicharts through DDE server and then visualize data in Multicharts and execute the trades using broker API or web/windows automation.

My code here will work on local feed and will give you voice alert as well. just download the file data_alert.wav from the repo and change the filename accordingly.

Important: Plot the chart in tick or seconds format in MultiCharts and then apply the indicator. Since it uses the last few bars, set bars back setting to a few thousand so it wouldn't hog the resources.
