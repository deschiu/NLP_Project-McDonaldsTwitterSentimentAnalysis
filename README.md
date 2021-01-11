# Social Listening on Twitter using Natural Language Processing (NLP)

This repository contains all the code to conduct sentiment analysis, on Tweets related to 'McPlant' - McDonald's new plant-based burger, using Tweepy, a Python library for accessing the Twitter API.

<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/intro.png" width="800"/>



**Business Value of this Project**

To discover all mentions and sentiments related to McDonald’s new burger product on Twitter, for instant Brand Reputation and Competitive Analysis.

It also offers valuables insights into Marketing Strategies, Product Development and Crisis Detection.

## What is in this repo?

* `Graph` contains all the visualizations made for analysis of sentiment and most popular topics.
* `data` contains csv files that store dataframes with cleaned tweets and relevant features.
* `main` contains notebooks that complete steps - from data acquisition, preprocessing, visualisation, transfer learning of LSTM model. 
* `LSTM_TwitterSentiment` contains a notebook that train the full LSTM model. 
* `TwitterListening_PPT.pdf` is a powerpoint which illustrates the complete framework of this project.



## How did we collect the data?
We used Tweepy, an easy-to-use Python library for accessing the Twitter API, and passing in relevant parameters such as - search words, language and number of tweets - to specify the items returned. 

The search words represent the areas we would like to analyse on: McDonald's and its biggest competitors, plant-based meat market and the plant-based product market.

<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/tweepy.png" width="800">

## What did we do the Text Cleaning?
We executed some common text pre-processing steps, and handle special cases at a later point to improve our results.

<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/txt-preprocessing.png" width="800">

## Language Model Training
### Dataset
We used Sentiment-140 dataset from Kaggle. It contains a labelled data of 1.6 million tweets and we found it a good amount of data to train our model.
</br>
<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/lstm01.png" width="800">

### Word Embedding
In language models, words are represented in a way to intend more meaning for pattern and contextual learning.Word Embedding is one of the popular representation of document vocabulary, which is capable of capturing context, semantic similarity of a word, and its relation with other words.

After text preprocessing, we applied transfer learning of GloVe, one of the pre-trained word embedding for word classification.

<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/lstm02.png" width="800">
Finally adopted LSTM Model with 3 epochs trained, which performed highest validation accuracy and least loss.

## Analysis
<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/mcd_sentiment-breakdown.png" width="800">
<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/mcplant_sentiment-over-time.png" width="800">
<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/mcplant_most-liked.png" width="800">
<img src="https://github.com/sophiachann/NLP-SocialListening-Twitter/blob/main/img/mcplant_summary.png" width="800">
