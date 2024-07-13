# Hate-Speech-Detection
# Analysis of Tweets for Hate Speech

This project analyzes tweets to detect hate speech and offensive language using various machine learning techniques. The primary goal is to preprocess the data, perform exploratory data analysis (EDA), build models, and evaluate their performance.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Conclusion](#conclusion)
8. [Future Work](#future-work)

## Introduction

This project aims to classify tweets into three categories: hate speech, offensive language, and neither. The dataset used for this analysis is publicly available and consists of tweets labeled by multiple users.

## Dataset

The dataset contains tweets with the following attributes:
- `hate_speech`: A count of the number of users who believe the tweet contains hate speech.
- `offensive_language`: A count of the number of users who believe the tweet contains offensive language.
- `neither`: A count of the number of users who believe the tweet is neither offensive nor contains hate speech.
- `tweet`: The text of the tweet.

## Data Preprocessing

Data preprocessing involves the following steps:
- Removing unnecessary characters, links, and punctuation from tweets.
- Converting text to lowercase.
- Tokenization and removing stop words.
- Lemmatization to reduce words to their base forms.

## Exploratory Data Analysis

Several visualizations and analyses are performed to understand the dataset better:
- Distribution of tweet classes.
- Frequency analysis of the labels assigned by the CrowdFlower users.
- Word cloud visualization for tweets.
- Top 20 words in tweets.
- Distribution of tweet lengths.
- Distribution of total user ratings.

## Modeling

Different machine learning models are built and evaluated:
- Logistic Regression
- Support Vector Machine (SVM)

## Evaluation

The performance of the models is evaluated using metrics such as accuracy, precision, recall, and F1-score. Additionally, ROC curves are plotted to compare the models' performance across different classes.

##Results

The performance of the models is as follows:

Logistic Regression:
Class 0 (AUC = 0.70): Moderate discriminative power.
Class 1 (AUC = 0.81): Good at distinguishing between class 1 instances and the rest.
Class 2 (AUC = 0.89): Performs very well in distinguishing between class 2 instances and the rest.

Support Vector Machine (SVM):
Class 0 (AUC = 0.66): Some ability to distinguish Class 0 from the rest.
Class 1 (AUC = 0.77): More effective at distinguishing Class 1 from the other classes.
Class 2 (AUC = 0.90): Strong ability to separate Class 2 instances from the rest.

## Conclusion

- Class 1 (offensive language) has a higher count within the dataset.
- Logistic Regression and SVM models have shown varying degrees of success in classifying tweets into the three categories.
- The models have demonstrated the ability to distinguish between the classes with varying AUC scores.

The analysis shows that the logistic regression model performs well in classifying tweets, especially for identifying hate speech and offensive language. The SVM model also performs adequately, particularly for classifying offensive language. These models can be further improved with more data and advanced feature engineering techniques.

## Future Work

Future improvements could include:
- Utilizing more advanced models like deep learning techniques.
- Enhance text preprocessing with advanced NLP techniques.
- Experiment with deep learning models such as LSTM and BERT for better performance.
