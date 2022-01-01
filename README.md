# Selected-3-Project

In this project we used data scrapped from https://www.arab-books.com/

First, We scrapped books data from the website like Book Name, Author, Category, Pages’ number, Dar El-Nashr, Book Size, and Description

Second, We cleaned the data from English words, numbers, and tags

Third, We used an autocorrect Library "Hunspell-ar" to correct mismatcched words        

Fourth, we stemmed and lemmatized the data using Faras, We tokenized, removed  the stop words, lemmatized and stemmed our data

Note:  We have tried different lemmatizers and stemmers (e.g. Qalsadi, Snowball stemmer, ISRI stemmer and Madamira) but we have found that Farassa has outperformed all of them on Arabic words.

Fifth, we train the model using RandomForestClassifier (RFC) on the features(description column) and labels(category column) after applying TF-IDF vectorizer then evaluated and tested the model on 30% of the dataset using new unseen data and achieve an accuracy of 73%.
