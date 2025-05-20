### Predicting tommorow's Bitcoin price.

**Author**
Shawn Arney

#### Executive summary

#### Rationale
Forecasting Bitcoin’s future value is crucial for safeguarding one’s investments in Bitcoin.

#### Research Question
Predicting tomorrow's closing price for Bitcoin.

#### Data Sources
Data sources include Bitcoin historical pricing data. 

Providing Bitcoin historical prices, volume data, and the funding rate for Bitcoin (Binance Futures, cost to borrow Bitcoin).  

*Including these data sources:*
Bitcoin Historical Data:
- https://github.com/ff137/bitstamp-btcusd-minute-data

Additional Funding Rate Data, from Binance Futures API:
- https://github.com/jesusgraterol/binance-futures-dataset-builder

#### Methodology
Bitcoin price prediction was approached from many different angles.  By exploring various regression models using supervised learning.  

And by using gridsearchCV with cross validation of 5, to tune parameters for evaluated models.  And neg_mean_absolute_error and mean_absolute_error was used for model evaluation.

*And includes:*

**Data Cleanup and Feature Selection:**
- Data Import from CSV Data Sources and Exchange API's
- Data cleanup, including dropping duplicates and setting Null values to 0
- Data aggregation of bitcoin minute data to daily data
- Data Feature Engineering columns 
- Data is split into training and test splits, with 20% set aside for testing
- And Data is encoded with a standard scaler for model processing

**Analysis includes:**
- Variance-Covariance matrixes to determine correlations with column features
- Cross Validation of 5 and neg_mean_absolute error and mean_absolute_error for model evaluation

**Models Evaluated Include:**
- Sarimax
- GridSearchCV for:
    - Support Vector Regression 
    - Linear Regression 
    - Ridge Regression
    - Lasso Regression 
    - Random Forest Regressor
    - Gradient Boosting Regressor
    - XGBoost Regressor
- Hyperband tuner for: 
    - Long Short-Term Memory (LSTM) Model

#### Results
Predicting tomorrow's closing price of Bitcoin, for a daily time frame.

Initial Model using SARIMAX has a Mean Absolute Percentage Error (MAPE) of 1.77%.
The Mean Absolute Error (MAE) is 898.27.

Our initial model, has an error rate within $898.27 US Dollars.

![sarimax](images/sarimax_results.png)

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Bitcoin Notebook](https://github.com/shawnarneygit/ai_machine_learning/blob/master/bitcoin/bitcoin.ipynb)

##### Contact and Further Information
Shawn Arney
Shawn@ArneyConsulting.com

https://www.linkedin.com/in/shawnarney/
