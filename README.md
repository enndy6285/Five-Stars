# Five Stars - NLP Analysis of Yelp Reviews

## Overview
Yelp is one of the largest platforms for customer generated business reviews with over 211 milion cumulative reviews to date. This wealth of information is valuable not to consumers but the businesses themselves. The Yelp rating can also have significant financial impact. A five star rating is the goal of every restaurant but what distinguishes a 5-star restaurant?

## Objective
Use NLP techniques to analyze Yelp text reviews to gain insight on features that are predictive of a 5-star rating.

## Methodology
### Data
Data was obtained from the Yelp Open Dataset available at https://www.kaggle.com/yelp-dataset/yelp-dataset. It was uploaded into MongoDB. A subset consisting of Toronto restaurant reviews was then downloaded for analysis
### NLP
Review text data was processed with NLTK tools including SnowballStemmer. Vectorization was performed with TF-IDF. Finally topical modeling was performed using NMF.
### Classification
The final topic models were used as features in a binary classification model with the target being a 5-star rating.

## Results
Using NLP tools, 50 topics were extracted from Yelp reviews text data. These were utilized in a logistic regression model to obtain feature importance. While there is a good amount of overlap between the topics, food and service appear to have the most impact on obtaining a 5-star rating. On the opposite end, long wait times predict not having 5 stars.

## Project Files
1. readme.md - project summary
2. five_stars_nlp.ipynb - Jupyter Notebook for NLP analysis
3. five_stars_data.ipynb - Jupyter Notebook for data collection using MongoDB and AWS
4. yelp_rest_toronto.pkl - dataframe of Toronto restaurant yelp reviews
5. five_stars_slides.pdf - Google slides presentation

