# Text-Classification

Naive Bayes classifiers are a collection of classification algorithm based around Baye's Theorem.

Naive Bayes classifiers have been heavily used for text classification and text analysis machine learning problems.

## Baye's Theorem
We are given a target vector _y_ and data matrix _X_, then:

![image](https://user-images.githubusercontent.com/77683275/150163839-f05214d3-e330-46a5-803f-422fa9a007b6.png)

## Data cleaning and pre-processing

We have to do this process no matter what way are we going to implement NaiveBayes (inbuilt sklearn classifer or self-implemented)

1. Go thorugh all data
2. Within a document go through all words
3. Ignore a word if its a stop word ('I', 'the', 'am', etc.,)
4. Add the word in dictionary with count 1, if not already present 
5. Else increase frequency of that word in the dictionary
6. Choose top k words (words with highesht frequency) as your features
7. Now create an np zero array of size = Num of Documents * No. of features(words in dictionary we creaated)
8. Set features as column header and in this 2D-array we will increment the frequency.

More Detailed and clear instruction to do this is written in comments within the Text Classification.ipynb

## Classifying Text using Naive Bayes

1- Using Inbuilt sklearn NaiveBayes MultinomialNB classifier

2- Self Implementation of Naive Bayes 

## Datasets

Dataset Used : http://archive.ics.uci.edu/ml/datasets/Twenty+Newsgroups
