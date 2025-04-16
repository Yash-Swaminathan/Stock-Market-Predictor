# Stock Price Prediction using LSTM

## Overview

This project implements a Long Short-Term Memory (LSTM) neural network to predict stock prices based on historical closing price data. It fetches historical data from Yahoo Finance, preprocesses and scales it, trains the model using a 60-day window, and visualizes actual vs. predicted prices.

## Features

- Fetches historical stock data using Yahoo Finance
- Scales and reshapes data for LSTM input
- Builds and trains a stacked LSTM model
- Tests and evaluates model accuracy on recent data
- Predicts the next day's closing price
- Visualizes actual and predicted prices using matplotlib

## Requirements

Install the necessary dependencies using pip:

```bash
pip install numpy pandas matplotlib pandas_datareader scikit-learn tensorflow
```
## Usage
1. Clone the repository or copy the script.

2. Change the stock ticker symbol in the script if needed:

3. Run the Python script:
```bash
python stock_predictor.py
```
This will:

Download stock data from 2012 to 2024

Train an LSTM model using a 60-day sliding window

Evaluate the model on 2024+ data

Plot the actual vs. predicted closing prices

Print the predicted price for the next trading day

## Notes

Only the closing price is used as input for simplicity.

The training window (prediction_days) is set to 60 by default.

The model uses 3 stacked LSTM layers with dropout to prevent overfitting.

The prediction is based on the most recent 60 days of data available.

Author
