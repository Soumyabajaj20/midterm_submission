# midterm_submission

it includes the codes of the programs whose main objective are :-
- Collect real-world financial news from RSS/XML feeds
- Parse and structure unstructured XML data
- Collect historical stock price data using an API
- Align news data with market trading days
- Reason about missing values and non-trading days
- Perform basic exploratory analysis
---
in the 
``` midterm_submission.ipynb ``` 
every code is given

First, i extracted the news from Yahoo Finance and stored source,headline and pubtime of the news and saved it in
```
news_raw.csv
```
then i changed the pubdate to the UTC timezone and timestaps to the the given format and included date and headline lenght coloumn to the news_raw.csv file and saved it as
```
news_cleaned.csv
```
---
then i choose NVDA (NVIDIA corporation) as a US listed stock and extracted it's details of open, high, low, close, volume of 10 trading days through yfinance
and the saved the file as 
```
stock_data.csv
```
then i merged the data with the stock listing and find out whether the nws day was a trading day or not and then saved the file as
```
merged_midterm_data.csv
```
then i made the plot of two insights which were news volume per day and the news distribution across sources.

then i did the sentiment analysis of all the headlines and got it's output either as positive, negative or neutral through finbert
---
```
news_with_sentiment.csv
```
then i edited this csv to get the new coloumn as target to as it is today's closing price - yesterday's closing price
```
news_with_sentiment_final.csv
```
then i trained the model of linear regression and random forest to get the output as predicted value of y and then for results i compared the models final value to target value to determine accuracy
```
model_performance_stats.csv
```
