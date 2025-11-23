# Multivariate-Crypto-Forecasting

This project implements a sophisticated, multivariate time-series forecasting model using a Long Short-Term Memory (LSTM) neural network built with TensorFlow/Keras. The goal is to predict the next-day closing price of Bitcoin (BTC-USD) by leveraging a rich set of financial features.

The model architecture utilizes a sequential design with two 50-unit LSTM layers, integrating 20% Dropout for regularization. It uses 'Close', 'Volume', 'High', and 'Low' price data, which is significantly enhanced through feature engineering by incorporating Log Returns (for stationarity/volatility) and Simple Moving Averages (20-day and 50-day) for momentum.

The data is rigorously preprocessed using MinMaxScaler for normalization and is split chronologically for training and testing. The model is compiled with the adam optimizer and mean squared error (MSE) loss. Performance is validated using industry-standard metrics, Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE), with visualizations provided to compare actual and predicted prices, as well as monitor training loss convergence.
