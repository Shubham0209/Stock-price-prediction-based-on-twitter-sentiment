# Stock-price-prediction-based-on-twitter-sentiment


### Project Description:

This project is about analyzing social media data about Apple Inc. and predicting its future stock trend with sentiment classification.
Sentiment analysis and machine learning principles were used to discover the possible effect of "public sentiment" on stock price.


### Data Preprocessing

1. Twitter data from [Kaggle](https://www.kaggle.com/nadun94/twitter-sentiments-aapl-stock)  for Apple stock was used for sentiment analysis. The time frame chosen to analyze data is `January 01, 2016` to `september 02, 2019`.   
    
2. Apple stock data was collected for the same time period from [Yahoo Finance](https://finance.yahoo.com/quote/AAPL/history?p=AAPL) for historical data analysis and stock price prediction.

3. Twitter information was processed to use only data for the dates the stock market was open (approximately 252 trading days per year).

4. Twitter Data and Daily stock prices were merged together and a final csv (Sentiment_polarity_AAPL.csv) was generated which was used as base data. For all the predictive analyses, I have used the adjusted close price of AAPL.

### Model training and evaluation

Different machine learning techniques were used to train and evaluate models to analyze and determine the correlation between twitter sentiment and Apple stock price. 


    Algorithms used for analysis:

    **Random Forest Regressor**

    Random Forest Regression is a supervised learning algorithm that uses ensemble learning method for regression. Ensemble learning method is a technique that combines predictions from multiple machine learning algorithms to make a more accurate prediction than a single model.


    **LSTM RNN**

    Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) architecture used in the field of deep learning. LSTM networks are well-suited for making predictions based on time series data, since there can be lags of unknown duration between important events in a time series.

    **XGBoost Regressor**

    XGBoost is short for Extreme Gradient Boosting and is an efficient implementation of the gradient boosting machine learning algorithm.


### Limitations/ What could have been done differently?

1. Twitter API has limitations on the amount of data that can be accessed. Therefore, a document with Twitter information regarding Apple stock from Kaggle was used.

2. NewsAPI headlines besides Twitter could also have been used for sentiment analysis.

3. Identifying optimum hyperparameters to fine tune the model outputs.


