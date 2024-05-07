# Stock Sentiment Analysis

This project uses the FinBERT model to perform sentiment analysis on news articles for a given list of stock tickers.

## Files

- `Main_testing.ipynb`: This is the main file where the sentiment analysis is performed.

## Functions

- `get_ticker_news_sentiment(ticker)`: This function takes a stock ticker as input and returns a DataFrame with the most recent news article headlines for that ticker, along with the overall sentiment of each article. The sentiment is determined using the FinBERT model.

- `generate_csv(ticker)`: This function takes a stock ticker as input and generates a CSV file with the most recent news article headlines for that ticker, along with the overall sentiment of each article.

## Usage

First, get a list of undervalued stocks using the `get_filtered_stocks()` function. Then, for each stock in the list, call the `get_ticker_news_sentiment(ticker)` function to get the sentiment of the most recent news articles for that stock.


## Dependencies
- pandas
- yfinance
- Goose
- transformers
- nltk

To install the dependencies, uncomment the first block, i.e. running this in Jupyter notebook will get the finvizfinance package installed:
- '%pip install finvizfinance'