# Stock Price Prediction using Sentiment Analysis and LSTM

## Overview

This project implements a stock price prediction model using **Long Short-Term Memory (LSTM)** networks and sentiment analysis based on financial news articles. The model is trained using historical stock price data combined with sentiment scores extracted from the news headlines. The goal is to predict the future stock prices by leveraging past prices and sentiment signals from news articles.

## Features

- **Sentiment Analysis**: Utilizes **FinBERT** (a model specifically fine-tuned for financial sentiment analysis) to classify news articles into positive or negative sentiment.
- **LSTM Model**: The core of the price prediction is done using an LSTM model, which excels at modeling sequential time-series data like stock prices.
- **Data Source**: Historical stock price data for Apple Inc. (AAPL) is sourced from Yahoo Finance using the `yfinance` API, while financial news headlines are scraped from Yahoo Finance.
- **Evaluation**: The model is evaluated based on the **Mean Squared Error (MSE)** and **R-squared** scores.

## Dataset

- **Stock Price Data**: The stock data is fetched from Yahoo Finance for the specified date range (2023-01-01 to 2023-12-31).
- **Sentiment Data**: News articles related to the stock are scraped from Yahoo Finance and analyzed using **FinBERT** to produce sentiment scores (positive or negative).

## Project Structure

- **data**: Contains the downloaded stock price data.
- **models**: The trained LSTM model and its configuration.
- **scripts**: Python scripts for data preprocessing, model training, and evaluation.
- **README.md**: This file.

## Requirements

To run this project, install the following dependencies:

```bash
pip install transformers yfinance pandas scikit-learn nltk keras tensorflow beautifulsoup4 requests matplotlib
