# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

Benjamin Toh, DSIF2

**Problem Statement**

To identify the right subreddit given a specific post

**Executive Summary**

This project will be utilizing Pushshift's API. I will collect posts from two subreddits which are from 'NBA' and 'PremierLeague' and identify which subreddit a given post belongs to. In order to achieve this, I will be using NLP to train a classifier to predict and classify the post to the correct subreddit. Two models will be created and compared where I will be using Naive Bayes and Random Forest classifier.


Preprocessing of the data are done via Tokenizing to split a string into substrings and remove special characters, Lemmatizing to shorten words by combining similar forms of the same word and CountVectorizer where it transform a given text into a vector based on the frequency it appears in the whole text.


Modeling was done through train test split, fitting the train data set in the model and prediction on the test data set. Hyperparameter tuning was performed on Random Forest Classifier. Both the models were compared using F1 scores, Accuracy scores and AUC values.


**Conclusions and Recommendations**

Based on the two models, Naive Bayes is the better model with higher F1 score, accuracy score and AUC value. However, Random Forest Classifier has a better consistency as it is a better fitted model. Future work like gathering more data and try out the TF-IDF Vectorizer will be carry out to build a more accurate model, I will also be removing majority of the common words which have high freqneucy of occurence. Other models like Logistic Regression, SVM, etc will be use as well, to further compare and decide on the best model for this binary classification.
