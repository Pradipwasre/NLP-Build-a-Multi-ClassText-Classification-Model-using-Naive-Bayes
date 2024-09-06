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


=== ====

# Multi-Class Text Classification with Naive Bayes

## Project Overview

This project implements the **Naive Bayes Algorithm** to build a multi-class text classification model. The goal is to classify customer complaints into different product categories using **Natural Language Processing (NLP)** techniques in Python.

## Example Calculation: Naive Bayes

### Problem Statement

We want to classify the sentence: **"This application is good."** into **"Positive"** or **"Negative"**.

### Training Data

| Sentence                         | Label    |
|----------------------------------|----------|
| "I love this app"                | Positive |
| "This app is great"              | Positive |
| "I hate the application"         | Negative |
| "The app is terrible"            | Negative |

### Prior Probabilities

- Total number of sentences = 4
- Number of Positive sentences = 2
- Number of Negative sentences = 2

\[
P(\text{Positive}) = \frac{2}{4} = 0.5
\]
\[
P(\text{Negative}) = \frac{2}{4} = 0.5
\]

### Likelihoods for Each Word

For the sentence **"This application is good."**, we calculate the likelihoods for each word given each class.

**Positive Class:**

- Vocabulary size (total unique words) = 7

\[
P(\text{"this"}|\text{Positive}) = \frac{1}{7}
\]
\[
P(\text{"application"}|\text{Positive}) = \frac{0 + 1}{7 + 4} = \frac{1}{11} \text{ (Laplace smoothing)}
\]
\[
P(\text{"is"}|\text{Positive}) = \frac{1}{7}
\]
\[
P(\text{"good"}|\text{Positive}) = \frac{0 + 1}{7 + 4} = \frac{1}{11} \text{ (Laplace smoothing)}
\]

**Negative Class:**

- Vocabulary size (total unique words) = 6

\[
P(\text{"this"}|\text{Negative}) = \frac{0 + 1}{6 + 4} = \frac{1}{10} \text{ (Laplace smoothing)}
\]
\[
P(\text{"application"}|\text{Negative}) = \frac{1}{6}
\]
\[
P(\text{"is"}|\text{Negative}) = \frac{1}{6}
\]
\[
P(\text{"good"}|\text{Negative}) = \frac{0 + 1}{6 + 4} = \frac{1}{10} \text{ (Laplace smoothing)}
\]

### Posterior Probability Calculation

**For Positive:**

\[
P(\text{Positive}|\text{"This application is good"}) \propto P(\text{"this"}|\text{Positive}) \times P(\text{"application"}|\text{Positive}) \times P(\text{"is"}|\text{Positive}) \times P(\text{"good"}|\text{Positive}) \times P(\text{Positive})
\]
\[
= \frac{1}{7} \times \frac{1}{11} \times \frac{1}{7} \times \frac{1}{11} \times 0.5
\]

**For Negative:**

\[
P(\text{Negative}|\text{"This application is good"}) \propto P(\text{"this"}|\text{Negative}) \times P(\text{"application"}|\text{Negative}) \times P(\text{"is"}|\text{Negative}) \times P(\text{"good"}|\text{Negative}) \times P(\text{Negative})
\]
\[
= \frac{1}{10} \times \frac{1}{6} \times \frac{1}{6} \times \frac{1}{10} \times 0.5
\]

### Comparison of Probabilities

Calculate the actual values:

**For Positive:**

\[
\frac{1}{7} \times \frac{1}{11} \times \frac{1}{7} \times \frac{1}{11} \times 0.5 \approx 0.00028
\]

**For Negative:**

\[
\frac{1}{10} \times \frac{1}{6} \times \frac{1}{6} \times \frac{1}{10} \times 0.5 \approx 0.00028
\]

Since both probabilities are very close, the sentence **"This application is good"** could be classified as **either Positive or Negative**. The exact classification might depend on additional factors or refinements in the model.
