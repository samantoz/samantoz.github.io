---
title: "Project 2: Stock Pick based on market data"
excerpt: "This project is to answer the question: Is it possible to build a dataset for a machine learning model that could learn the nature of a stock based on the company performnace and then leverage this knowledge in order to predict which stock will be worth buying?"
collection: portfolio
---
I have used 3 sources for my project. The first source is a csv file showing the data collected from 200+ financial indicators for all the stocks of the US stock market. The financial indicators have been scraped from Financial Modeling Prep API, and are those found in the 10-K filings that publicly traded companies release yearly.

- Name of the source is FinancialIndicators.csv

The second source is an API for the End Of Day Stock Prices.This is updated daily and this data feed offers end of day prices, dividends, adjustments and splits for US publicly traded stocks with history to 1996. Prices are provided both adjusted and unadjusted.
The Key Features of the dataset:  

   1. Covers all stocks with primary listing on NASDAQ, AMEX, NYSE and ARCA.  
   1. Includes unadjusted and adjusted open, high, low, close, volume.  
   1. Includes dividend history and split history.  
   1. Updated at or before 5:00pm ET on all trading days.  
   1. Exchange corrections are applied by 9:30pm ET.  
   1. Historical data goes back to 1996.  

The third source is the daily transaction for a ticker price chart from yahoo: www.finance.yahoo.com

I wanted to answer the question:

Is it possible to build a dataset for a machine learning model that could learn the nature of a stock based on the company performnace and then leverage this knowledge in order to predict which stock will be worth buying?
I used sqllite as my database and inserted all the 3 datasets into it. The joining criteria between the various datasets are date and ticker symbols of the stocks. I used 5 tickers for my analysis.
The process I followed is to insert the datasets into separate tables using a database and then using the database to join the datasets and bring the merged dataset into pandas dataframe and use the dataframes to generate the visuals.
The database was used to insert the data in the most native format without modifying any data types. All dataset was inserted as string values as that is the easiest way to represent the data in the database.

My learning form this project is that merging the data and making it useful for a data science analysis is a lot of hard work. In real life the source dataset is far from perfect. The data wrangling process should be made very robust in order to make the dataset meaningful and so that it could be used efficiently by the data analyst/scientist. The work of the data engineer here is very vital too in preparing the data for the data science analysis.

This is a link to the source code is [**here**](https://github.com/samantoz/bu-datascience/tree/master/DSC540-DW/Term_Project)
