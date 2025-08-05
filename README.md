# Mails Spam Detector

## Problem
There are so many unwanted spam messages or mails that waste time and disturb users. We need a simple way to automatically detect and filter these spam messages.

## Solution
This project solves that by training a model to classify whether a message or mail is spam or not using a Naive Bayes algorithm.

## What Are We Finding
We are predicting if a given text message or mail is spam (1) or not spam (0).

## Columns Used
We used the v1 column to get the labels (spam or ham), and v2 column for the message text. All other columns were dropped.

## Model Used
I used MultinomialNB from Naive Bayes, because it works great for text classification problems.

I also used a Pipeline to make things easier. This way, I don’t have to vectorize every input manually again and again. The pipeline does it all in one go: it converts text to numbers (CountVectorizer) and then applies the model.

## Accuracy
The final accuracy was 0.990667623833453 (almost 99%) on the test set.
