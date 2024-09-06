## Modular Code Structure of the Project

### *Project Directory*

### Modular_code/
- **Input/**: Contains input dataset.
  - `complaints.csv`: Customer complaints data.
  
- **Output/**: Stores generated models.
  - `count_vect.pkl`: CountVectorizer model saved after training.
  - `nb.pkl`: Naive Bayes model saved after training.
  
- **Source/**: Contains scripts for core functionality.
  - `model.py`: Script for training the model.
  - `processing.py`: Data preprocessing functions.
  - `utils.py`: Helper and utility functions.
  
### Additional Files
- **config.py**: Configuration settings for paths, etc.
- **Engine.py**: Main script to execute the project workflow.
- **naive_bayes.ipynb**: Jupyter notebook for testing and development.
- **predict.py**: Script for making predictions.
- **README.md**: Documentation and project overview.
- **requirements.txt**: Dependencies for Python libraries.
  
### Data Files
- **nltk_data/**: Data files from NLTK for text processing.

---------------------------------------------------------------

## Folder Structure

- **Modular_code/**
  - **Input/** (CSV): `complaints.csv` — Dataset for consumer complaints.
  - **Output/** (PKL): `count_vect.pkl`, `nb.pkl` — Saved models for reuse.
  - **Source/** (PY):
    - `model.py` — Script for training the Naive Bayes model.
    - `processing.py` — Data preprocessing utilities.
    - `utils.py` — Helper methods.
  - **config.py** — Configuration file with file paths.
  - **Engine.py** — Main script to run the entire workflow.
  - **naive_bayes.ipynb** (IPYNB) — Jupyter Notebook for interactive work.
  - **predict.py** — Script for generating predictions from trained models.
  - **README.md** — Project documentation.
  - **requirements.txt** — Dependencies for the project (Python libraries).
  - **nltk_data/** — Directory for NLTK data such as stopwords.

---------------------------------------------------------------

# NLP Multi-Class Text Classification with Naive Bayes

## Overview

Welcome to the NLP Multi-Class Text Classification project! This repository showcases how to build an efficient text classification model using the Naive Bayes algorithm. The model is designed to categorize customer complaints into predefined classes, streamlining the process of handling and analyzing customer feedback.

## Project Motivation

In the world of customer service, handling large volumes of customer complaints efficiently is crucial. This project aims to automate the categorization of these complaints into specific classes, such as "Billing", "Service", and "Technical Issue", allowing companies to quickly address and analyze customer issues.

By employing the Naive Bayes algorithm, known for its simplicity and effectiveness in text classification tasks, we provide a robust solution to manage and understand customer feedback at scale.

## Naive Bayes Algorithm

Naive Bayes is a probabilistic classification technique based on Bayes' Theorem with an assumption of independence among features. Here’s why it's effective:

- **Bayes' Theorem**: Calculates the probability of a class given the presence of features in the data. The theorem is expressed as:
  \[
  P(C|X) = \frac{P(X|C) \cdot P(C)}{P(X)}
  \]
  Where:
  - \(P(C|X)\) is the posterior probability of class \(C\) given features \(X\).
  - \(P(X|C)\) is the likelihood of features \(X\) given class \(C\).
  - \(P(C)\) is the prior probability of class \(C\).
  - \(P(X)\) is the evidence or the probability of features \(X\).

- **Feature Independence**: Assumes that features are independent given the class, simplifying calculations and making the algorithm efficient.

- **Types of Naive Bayes Classifiers**:
  - **Multinomial Naive Bayes**: Best suited for text classification where features are word counts.
  - **Bernoulli Naive Bayes**: Suitable for binary/boolean features.
  - **Gaussian Naive Bayes**: Ideal for continuous features.

Despite its simplicity, Naive Bayes often yields excellent results, especially for large text datasets.

## Project Structure

Here’s a breakdown of the project files and their purpose:

### Modular_code/
- **Input/**: Contains input data.
  - `complaints.csv`: Dataset with customer complaints.

- **Output/**: Stores trained models and vectorizers.
  - `count_vect.pkl`: Serialized CountVectorizer object.
  - `nb.pkl`: Serialized Naive Bayes model.

- **Source/**: Core scripts for functionality.
  - `model.py`: Script for training the Naive Bayes model.
  - `processing.py`: Functions for data preprocessing.
  - `utils.py`: Utility functions for saving and loading models.

### Additional Files
- **config.py**: Configuration file for paths and settings.
- **Engine.py**: Main script to execute the end-to-end workflow.
- **naive_bayes.ipynb**: Jupyter notebook for exploratory analysis and testing.
- **predict.py**: Script for making predictions on new complaints.
- **README.md**: Documentation file for the project.
- **requirements.txt**: File listing project dependencies.

### Data Files
- **nltk_data/**: Contains data files for NLTK, used for text processing.

## Getting Started

To get started with this project, follow these steps:

1. **Install Dependencies**: Run `pip install -r requirements.txt` to install all necessary libraries.
2. **Prepare Data**: Ensure that your `complaints.csv` file is in the `Input/` directory.
3. **Train the Model**: Execute the training script with `python Engine.py`. This will process the data, train the Naive Bayes model, and save the results.
4. **Make Predictions**: Use `python predict.py --test_complaint "your complaint text here"` to classify new complaints.

## Contributing

Contributions to this project are welcome! If you have suggestions for improvements or find issues, please submit a pull request or open an issue on the GitHub repository.


## Contact

For any questions or feedback, please contact [https://www.linkedin.com/in/pradip-wasre/].

---

Thank you for checking out the NLP Multi-Class Text Classification project. We hope you find it useful and informative!

