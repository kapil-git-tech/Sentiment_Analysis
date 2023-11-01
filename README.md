# This repository has a couple of use cases on SENTIMENT ANALYSIS:

### 1. Sentiment Analysis for "AAPL" using twitter data - VADER Sentiment Analysis on Yearly data (2018)
### 2a. Sentiment Analysis on Apple phone reviews on Amazon using BERT
### 2b. Comparison of results between BERT & VADER

The 1st notebook examines the relationship between twitter sentiment and stock price.

Part A of the first notebook focusses on sentiment analysis.

- I have used NLTK's built-in, pretrained sentiment analyzer VADER (Valence Aware Dictionary and sEntiment Reasoner).
The pre-trained sentiment analyzer returns the 'compound' score for each tweet. This score ranges from -1 (most negative) to +1 ( most positive).

Part B of the first notebook establishes the relationship between twitter sentiment & stock price

- I have downloaded the stock data for Apple from yfinance.

[View the Notebook on GitHub repository](https://github.com/kapil-git-tech/Sentiment_Analysis/blob/main/sentiment-analysis-with-twitter-data-for-apple.ipynb)

The 2nd notebook uses the pre-trained BERT based uncased model and fine-tunes it with Apple reviews data on Amazon.
- I have tried the base & large cased as well as uncased model during training but left the results of the base uncased model in the notebook as it gave better results.
The fine-tuned model is tested on a holdout sample & the results are shared. All the details related to fine-tuning are provided in detail in the notebook.
The notebook can be used to fine tune the model for different use cases & hyperparameters can be modified to uplift accuracy.

[View the Notebook on GitHub repository](https://github.com/kapil-git-tech/Sentiment_Analysis/blob/main/sentiment-analysis-on-phone-reviews-bert-use-case.ipynb)

The 3rd notebook just appends the results from VADER towards the end of notebook 2. The notebook proves how BERT fine tuned model is better at predicting sentiment than VADER.

View the Notebook on GitHub repository](https://github.com/kapil-git-tech/Sentiment_Analysis/blob/main/sentiment-analysis-on-phone-reviews-bert-vs-vader.ipynb)