<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stock Data Analysis with Reddit Integration</title>
</head>
<body>
    <h1>Stock Data Analysis with Reddit Integration</h1>
    <p>This project performs stock data analysis using data sourced from Yahoo Finance, Naver, and Stooq, and demonstrates how to integrate Reddit API to retrieve posts and comments. Additionally, it extracts financial data from various online sources and analyzes stock prices over a specific time range. The script also plots the stock prices and trading volumes.</p>

    <h2>Key Components</h2>
    <ul>
        <li><strong>Reddit API Integration:</strong> Using PRAW (Python Reddit API Wrapper) to fetch and display subreddit posts and comments from the <em>r/datascience</em> subreddit.</li>
        <li><strong>Web Scraping:</strong> BeautifulSoup is used to scrape code examples from the <em>Pandas DataReader</em> documentation.</li>
        <li><strong>Stock Data Retrieval:</strong> Data is fetched from Yahoo Finance, Naver, and Stooq using <em>yfinance</em> and <em>pandas_datareader</em>.</li>
        <li><strong>Data Visualization:</strong> Stock data (Open, High, Low, Close prices) and volume traded are visualized using Matplotlib.</li>
        <li><strong>Important Price Levels:</strong> Functions to identify key support/resistance levels, high volatility regions, and high volume areas for each stock.</li>
    </ul>

    <h2>Libraries Used</h2>
    <ul>
        <li>PRAW</li>
        <li>BeautifulSoup</li>
        <li>Pandas</li>
        <li>Yfinance</li>
        <li>Pandas DataReader</li>
        <li>Matplotlib</li>
        <li>NumPy</li>
    </ul>

    <h2>Installation and Setup</h2>
    <ol>
        <li>Install the required Python libraries:
            <pre><code>pip install praw beautifulsoup4 pandas yfinance pandas-datareader matplotlib numpy configobj</code></pre>
        </li>
        <li>Create an <code>.env</code> file to store your Reddit API credentials:
            <pre><code>
REDDIT_CLIENT_ID='your_client_id'
REDDIT_CLIENT_SECRET='your_client_secret'
REDDIT_USERNAME='your_username'
REDDIT_PASSWORD='your_password'
            </code></pre>
        </li>
        <li>Run the Python script to fetch stock data, analyze it, and visualize the results.</li>
    </ol>

    <h2>Usage</h2>
    <ol>
        <li>The script starts by connecting to the Reddit API using your credentials and fetches posts from the <em>r/datascience</em> subreddit.</li>
        <li>It extracts stock data from Yahoo Finance, Naver, and Stooq for a given date range.</li>
        <li>Stock price and volume are plotted for comparison among different sources.</li>
        <li>The script identifies important price levels such as highest and lowest prices, mean price, volatility, and volume statistics.</li>
    </ol>

    <h2>Output Examples</h2>
    <p>Stock price charts and volume comparisons for Yahoo, Naver, and Stooq sources, as well as statistical analysis of important price levels.</p>
</body>
</html>
