# Stock-Price-Prediction-Using-LSTM
# Apple Stock Price Prediction Using LSTM

This project demonstrates how to predict the closing stock prices of Apple Inc. (AAPL) using a Long Short-Term Memory (LSTM) neural network.

## Overview

- We download historical stock price data for Apple using the `yfinance` library.
- The data is preprocessed by scaling the closing prices between 0 and 1.
- Using a window of 60 previous days’ closing prices, we train an LSTM model to predict the next day’s closing price.
- The model consists of two LSTM layers followed by Dense layers for regression output.
- After training, the model is tested on the most recent 5% of the data.
- Predictions are inverse-transformed to original scale and evaluated using Root Mean Squared Error (RMSE).
- Visualizations include price history plots, moving averages, and prediction performance.

## Features

- Downloads and preprocesses 10+ years of daily closing price data for Apple Inc.
- Scales data with `MinMaxScaler` to enhance LSTM training.
- Uses a sliding window approach with 60 days sequence input.
- Builds a stacked LSTM model with 128 and 64 units.
- Predicts future closing prices and compares them with actual values.
- Calculates error metrics and visualizes results for interpretation.

## Dependencies

- Python 3.x
- numpy
- pandas
- matplotlib
- seaborn
- yfinance
- scikit-learn
- tensorflow / keras

## Usage

- Run the Python script to download data, train the LSTM model, and plot predictions.
- Modify date ranges or stock ticker symbols as needed.
- Tune LSTM parameters like number of layers, units, epochs, and batch size for improved performance.

## Results

- The trained model achieves an RMSE value indicating the average prediction error.
- Visualization plots help analyze the closing price trends and prediction accuracy.

## Future Work

- Extend to multi-stock predictions or portfolio analysis.
- Integrate more features such as volume, technical indicators, or news sentiment.
- Experiment with more complex models or hyperparameter tuning.
