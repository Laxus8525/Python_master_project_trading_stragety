# Python_master_project_trading_stragety
Bulid three types of trading stragety, momentum stragety, mean reversion stragety, and machine learning stragety to invest S&amp;P 500 from November 2003 to October 2022 to make more profit than buy and hold S&P500.
In momentum stragety, I used short, mid, and long period simple moving average cross method to find the buy and sell potins. Mean reversion strategy was used to find extreme suitation of stock markets. And I used for loop to find best parameters of these two strategy.
In machine learning strategy, Kmeans algorithm was used to split the market into two types, bullish market and bearish market. I use daily volume and daily price change range represented by ( High - Low)/ Close to sort the suitation of SP500 daily price. We set bullish market as 1 and bearish market as -1 as target value for the next prediction step. The features are daily price change, inday price change, inday price-volume relationship (High - Low)/Volume, long-term trend (under 180-days simple moving average price going up, 60-days simple moving average price above 90-days simple average moving average price as 1, other as -1) and extreme drop (when close price is below 250-days expotential moving average price minus 1.5 times 120-days expotential moving average volalitity). The size of the train set is 80% of data. I use models of Classification family and use the accuracy metric to evaluate the models. Next, I will select the most suitable model and do hypertuning to predict the suitation of SP500. If the predicted value is 1, I will hold the long position wheras hold short position. And use quantstats to generate performance reports for mean reversion and momentum stragties comapring the benchmark SP500.
