# Arabic NLP

In this project we used data scrapped from https://www.arab-books.com/

First, We scrapped books data from the website like Book Name, Author, Category, Pages’ number, Dar El-Nashr, Book Size, and Description.

Second, We cleaned the data from English words, numbers, and tags.

Third, We used an autocorrect Library "Hunspell-ar" to correct mismatcched words.

Fourth, we stemmed and lemmatized the data using Farassa, We tokenized, removed  the stop words, lemmatized and stemmed our data.

Note:  We have tried different lemmatizers and stemmers (e.g. Qalsadi, Snowball stemmer, ISRI stemmer and Madamira) but we found that Farassa has outperformed all of them on Arabic words.

Fifth, we train the model using RandomForestClassifier (RFC) on the features(description column) and labels(category column) after applying TF-IDF vectorizer then evaluated and tested the model on 30% of the dataset using new unseen data and achieved an accuracy of 73%.

Sixth, we created two Question-Answer Datasets, then we matched the input query with the questions in the two Datasets and retrieved the most relevant answer.

Seventh, we weighted all the words of All Descriptions of the books, we weighted the important keywords by calculating Tf-Idf for each one.
Note: We removed all stop words from the Descriptions.
