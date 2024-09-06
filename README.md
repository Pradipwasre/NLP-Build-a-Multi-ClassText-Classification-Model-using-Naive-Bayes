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

----------------------------------------------------------------------

## Project Features

Data Exploration: Visualizing customer complaint data to identify patterns.
Text Preprocessing: Applying techniques such as lowercasing, tokenization, stopword removal, and punctuation removal.
Model Building: Training a Naive Bayes classifier using the Scikit-learn library.
Model Evaluation: Measuring the model's accuracy on test data.
Predictions: Using the trained model to predict product categories for new complaints.

----------------------------------------------------------------------

## Tech Stack


Language: `Python`
Libraries:
`pandas`, `seaborn`, `matplotlib` for data analysis and `visualization`.

`nltk` for NLP tasks like tokenization and stopword removal.
`sklearn` for `Naive Bayes` model implementation.

----------------------------------------------------------------------

## Approach

Data Visualization: Explore and visualize the dataset to understand patterns.
Data Preprocessing:
Convert text to lowercase.
Tokenize the complaint texts.
Remove stopwords and punctuation.
Model Building: Train a Naive Bayes classifier for multi-class classification.
Model Evaluation: Evaluate the model's accuracy and performance on test data.
Predictions: Make predictions on new, unseen complaint reviews.

----------------------------------------------------------------------


### Naive Bayes Formula

The Naive Bayes algorithm is based on **Bayes' Theorem**:

**P(C|X) = [P(X|C) * P(C)] / P(X)**

Where:

- **P(C|X)**: Posterior probability of class C given the feature X.
- **P(X|C)**: Likelihood of feature X given class C.
- **P(C)**: Prior probability of class C.
- **P(X)**: Probability of the feature X (can be ignored for classification since it's constant).
sses, can be ignored for classification)

