# Forcast-euro-yen

This Python program aims to predict the market price of FOREX using time series analysis with ARIMA models. Here's a brief description of the code and its functionalities:

First, the necessary libraries are imported, such as pandas, numpy, matplotlib, seaborn, requests, datetime, timedelta, and statsmodels. Then, an API key is generated to get access to market data.

Next, the program requests historical data of the chosen currency pair (EUR/JPY) using the API and saves it as a pandas dataframe. The data is then cleaned and preprocessed, with the 'date' column converted to datetime format and set as the dataframe index.

The program then performs statistical analysis on the high prices of the currency pair, including a probability plot, ADF (Augmented Dickey-Fuller) test for stationarity, ACF (AutoCorrelation Function) plot, and PACF (Partial AutoCorrelation Function) plot.

Afterwards, the dataframe is split into training and testing datasets. The ARIMA model is then trained on the training dataset with the order parameter set to (2,1,2) and used to predict future prices of the currency pair.

Overall, this program provides a basic framework for implementing a time series analysis on FOREX data using Python.
