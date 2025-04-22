### Predicting the directional and future price of bitcoin.

**Author**
Shawn Arney

#### Executive summary

#### Rationale
Forecasting Bitcoin’s future value is crucial for safeguarding one’s investments in Bitcoin.

#### Research Question
Predicting the future price for bitcoin.  Firstly, predicting whether the bitcoin price will decline or increase in value, and for what time frames.  And secondly, predicting the actual future price of bitcoin, for a time frame.

#### Data Sources
Data sources include free and paid bitcoin historical data.  And may include additional data sets, as required.  

Providing bitcoin historical prices, volume data, technical indicators (RSI), open interest ratios, liquidity levels, the order book, on chain activity, options and their expirations, and market sentiment.  

Including these data sources:
- https://github.com/ff137/bitstamp-btcusd-minute-data
- https://finance.yahoo.com
- https://www.bybit.com/future-activity/en/developer
- https://hyblockcapital.com/api-explorer
- https://api.santiment.net

#### Methodology
Bitcoin price prediction will be approached from many different angles.  

And includes:

Data import and clean up from api's and csv data sources.

Variance-Covariance matrixes to determine correlations with features.

Time-series Forecasting.

Statistical on chain analysis of bitcoin flow, the order book, open interest, volume, and liquidity levels.  

News/Sentiment from X.com

Independent features for the day of week, time of day. Using auto regressive feature selection.

Sophisticated Indicators currently used for price prediction in trading.  Including RSI and The Demark(R) Indicator.

Exogenous Regression

GridSearchCV, Linear Regression

Support Vector Machine Models, and others as needed.

#### Results
Predicting the actual future price of bitcoin, for a daily time frame.

Initial Model using SARIMAX has a MAPE of 1.91%.

![sarimax](images/sarimax_results.jpg)

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Bitcoin Notebook](https://github.com/shawnarneygit/ai_machine_learning/blob/master/bitcoin/bitcoin.ipynb)


##### Contact and Further Information
Shawn Arney
Shawn@ArneyConsulting.com
