# Multi-Class Text Classification with Naive Bayes

**Project Overview**

This project implements the Naive Bayes Algorithm to build a multi-class text classification model. The goal is to classify customer complaints into different product categories using Natural Language Processing (NLP) techniques in Python.

----------------------------------------------------------------------

## What is Naive Bayes?

Naive Bayes is a probabilistic classification algorithm that applies Bayes' Theorem with the assumption that all features (words) are independent of each other. Despite this "naive" assumption, the model performs well for text classification tasks due to the high-dimensional nature of text data.

----------------------------------------------------------------------

## How Naive Bayes Works in NLP

1. Tokenization: Splitting the text into individual words (tokens).
2. Stopword Removal & Cleaning: Removing common words (like "and", "the") and punctuation to clean the text.
3. Word Frequency: Counting the occurrence of each word in the text for each class.
4. Class Probability Calculation: Using Bayes' Theorem to calculate the probability of a document belonging to a specific class based on word frequencies.
5. Prediction: The class with the highest probability is assigned to the document.
