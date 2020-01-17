# yelp-dataset

## Overview
In this repository I do some exploratory analysis of the Yelp dataset and take the opportunity to learn more about NLP by applying it to Yelp's 'review' data (reviews of businesses on Yelp). The project is a collection of notebooks. I use standard data science tools (pandas, matplotlib, sklearn, numpy) and some standard tools in NLP (nltk, word2vec). I explore the data, determine words and topics indicative of great and terrible reviews, segment users, segment reviews. 

## Ambition 
I am working to predict business categories with the ambition that I'll eventually build a Recommendation System to recommend business categories. This product would be used by business owners to label their business with appropriate categories that they are currently missing so that they can be discovered by more users on Yelp! This part is a work in process. 

## Exploratory
To date the project has a few completed analyses. Notebook 1 has an initial brainstorm, some data cleaning, and an analysis to determine words indicative of great (5-star) and terrible (1-star) reviews on Yelp (utilizing bag of words). I also do this using TFIDF instead of bag of words (Notebook 2). I extend this in Notebook 3 to topics indicative of reviews; I use NMF and LDA for the topic modeling. 

## User Segmentation
In Notebook 4 I use TFIDF to perform User (customer/reviewer) Segementation. I create WordClouds summarizing the vocabulary of these users types. In Notebook 5 I segment users using word2vec and again create WordClouds to summarize the user types. Word2vec is a sophisticated embedding and does a much better job of segmenting user types; the WordClouds allow you to understand the motivations of each customer segment much more clearly. For example, some users are interested in activity locations (casino/library/lake/theater/church), whereas several groups are intersted in food. The users with interest in food include segments that are interested in different aspects of the business. For example, one segment is interested in the food itself (delish/tasty/empanadas/cornbread/other-menu-items), whereas another segment is is more interested in the ambiance (ambiance/atmosphere/satisfying). 

## Review Segmentation
In Notebook 6 I use word2vec to segment reviews to understand the different types of reviews left on Yelp. The wordclouds give great insight into what reviews on Yelp discuss. 

## Category Prediction
In Notebook 7 I build a model to predict its business categories (Nightlife, Sports Bars, Shoe Repair, Seafood Market, Bowling, ...) using just the Yelp reviews of the business. I am working towards building a recommendation system for business categories. Eventually I'd like to produce a webapp so that a business owner can input their Yelp ID and get a recommended list of categories for their business on Yelp. If a business has missing category labels on Yelp then they are missing out on being discovered by Yelp users searching for those categories so this tool can add significant value for business owners. 

