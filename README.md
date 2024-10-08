# Stock Data Analysis with Reddit Integration

This project performs stock data analysis using data sourced from Yahoo Finance, Naver, and Stooq, and demonstrates how to integrate Reddit API to retrieve posts and comments. Additionally, it extracts financial data from various online sources and analyzes stock prices over a specific time range. The script also plots the stock prices and trading volumes.

## Key Components

- **Reddit API Integration:** Using PRAW (Python Reddit API Wrapper) to fetch and display subreddit posts and comments from the *r/datascience* subreddit.
- **Web Scraping:** BeautifulSoup is used to scrape code examples from the *Pandas DataReader* documentation.
- **Stock Data Retrieval:** Data is fetched from Yahoo Finance, Naver, and Stooq using `yfinance` and `pandas_datareader`.
- **Data Visualization:** Stock data (Open, High, Low, Close prices) and volume traded are visualized using Matplotlib.
- **Important Price Levels:** Functions to identify key support/resistance levels, high volatility regions, and high volume areas for each stock.

## Libraries Used

- PRAW
- BeautifulSoup
- Pandas
- Yfinance
- Pandas DataReader
- Matplotlib
- NumPy

## Installation and Setup

1. Install the required Python libraries:

    ```bash
    pip install praw beautifulsoup4 pandas yfinance pandas-datareader matplotlib numpy configobj
    ```

2. Create an `.env` file to store your Reddit API credentials:

    ```
    REDDIT_CLIENT_ID='your_client_id'
    REDDIT_CLIENT_SECRET='your_client_secret'
    REDDIT_USERNAME='your_username'
    REDDIT_PASSWORD='your_password'
    ```

3. Run the Python script to fetch stock data, analyze it, and visualize the results.

## Usage

1. The script starts by connecting to the Reddit API using your credentials and fetches posts from the *r/datascience* subreddit.
2. It extracts stock data from Yahoo Finance, Naver, and Stooq for a given date range.
3. Stock price and volume are plotted for comparison among different sources.
4. The script identifies important price levels such as highest and lowest prices, mean price, volatility, and volume statistics.

## Output Examples

Stock price charts and volume comparisons for Yahoo, Naver, and Stooq sources, as well as statistical analysis of important price levels.


