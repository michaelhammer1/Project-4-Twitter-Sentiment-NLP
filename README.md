## Twitter Sentiment Project Using NLP

By: Michael Hammer

#Overview
At a SXSW event, 9,000 Tweets were collected pertaining to Google, Apple and other sources. We analyzed Tweets about Apple and Google to build a model that will classify positive Tweets from Negative Tweets. 
We also analyze particular words that seem to stick out that Apple and Google teams can use to improve products and clean up their name.
The stakeholders: Google, Apple and other companies that want to see if a given Tweet is positive or negative.

# Goal
Use the dataset to build company sentiment model. Build a machine learning model with the inputs as the labeled tweets and sentiment of positive and negative as outputs.

# Data
data.world has a 9,000 tweet dataset about Google and Apple. The tweet labels reflect the emotion of the tweet and to which company it is referring.

# Methods
We started by preparing the data. We assigned company names by products. 

Then we did EDA and visualized the most common words using WordCloud. We made similar steps as NLP processing, tokenizing the tweets, removing customized stopwords, lemmitizing and vecotrizing with TfidfVectorizer.

Finally we modeled positive and negative tweets. We SMOTEd for the class imbalance and modeled with random forest and logistic regression. Then we used GridSearch to find the optimal parameters.

# Results
The best modele was a logistic regression model with an accuracy score of 0.88
Confusion matrix
[40 93
 9 742]

# Conclusions
Overall the dataset was 60.2% neutral/unsure emotion, 33.3% positive emotion and 6.4% negative emotion.

We saw that or Google people were discussing 'circle' and 'social' in both positive and negative tweets. Negative tweets contain words like 'false', 'alarm', 'wait', 'fail', and 'lost' much more than in positive tweets.

For Apple 'app', 'store' and 'Austin' show up with similar frequency in both positive and negative tweets. Positive tweets discussed 'ipad2' and 'free.' Likely people were reacting positively to free items Apple was giving out at the convention. Negative tweets highlight 'battery,' likely refering to poor battery lives of Apple products. 14 tweets referred to Apple as a 'facist company.' Finally people wrote negative tweets referring to 'fail,' 'fade,' 'hate,' 'headaches,' and 'Blackberry.'

# Next steps
Further investigate other models. Acquire more data. Find customers who want us to analyze tweets about their companies. Build a twitter scraper.
