# Social Listening on Twitter using Natural Language Processing (NLP)

This repository contains all the code to conduct sentiment analysis, on Tweets related to 'McPlant' - McDonald's new plant-based burger, using Tweepy, a Python library for accessing the Twitter API.

--> IMG - Sentiments, WordCloud

**Business Value of this Project**
<p>To discover all real-time mentions and sentiments on Twitter related to McDonald’s new burger product, for instant Brand Reputation and Competitive Analysis, offering valuables insights into Marketing Strategies, Product Development and Crisis Detection.</p>

## What is in this repo?

* `Graph` contains all the visualizations made for sentiment analysis and discovery on most-discussed topics.
* `data` contains csv files that store dataframes with cleaned tweets and corresponding features.
* `main` contains notebooks that complete steps from data acquisition, preprocessing, visualisation, transfer learning of LSTM model. 
* `twitter_sentiment_LSTM_model` contains notebook that train the full LSTM model. 



## How did we collect the data?
We used Tweepy, an easy-to-use Python library for accessing the Twitter API, and passing in relevant parameters, such as search words, language and number of tweets to specify the items returned. The search words represent the areas we would like to analyse on, which include McDonald's competitors, plant-based meat market and the plant-based product market.

--> IMG - Tweepy

## What did we do the Text Cleaning?
We executed some common text pre-processing steps, and handle special cases at a later point to improve our results.

--> IMG - Data Cleaning

## LSTM Model Training
--> IMG

