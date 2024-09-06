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

## Project Motive

The purpose of this project is to build a multi-class text classification model using the Naive Bayes algorithm. The goal is to develop a model that can automatically categorize customer complaints into predefined classes, making it easier for companies to handle and analyze large volumes of customer feedback.

Text classification is a common task in Natural Language Processing (NLP) that involves assigning predefined labels to text based on its content. In this project, we focus on classifying customer complaints into categories such as "Billing", "Service", "Technical Issue", etc.

By leveraging the Naive Bayes algorithm, this project aims to provide a simple yet effective solution for text classification. The Naive Bayes algorithm is known for its efficiency and effectiveness, particularly with text data, making it a suitable choice for this task.

## Naive Bayes Algorithm

The Naive Bayes algorithm is a probabilistic machine learning model based on Bayes' theorem, which is used for classification tasks. It assumes that the presence of a feature (in this case, a word or term) in a document is independent of the presence of any other feature. This assumption of independence is why the algorithm is termed "naive."

### Key Concepts

- **Bayes' Theorem**: This theorem calculates the probability of a class given the features (words) in a document. The formula is:
  \[
  P(C|X) = \frac{P(X|C) \cdot P(C)}{P(X)}
  \]
  Where:
  - \(P(C|X)\) is the probability of class \(C\) given the features \(X\).
  - \(P(X|C)\) is the probability of features \(X\) given class \(C\).
  - \(P(C)\) is the prior probability of class \(C\).
  - \(P(X)\) is the probability of features \(X\).

- **Feature Independence**: Naive Bayes assumes that all features are independent given the class. This simplifies the computation of the probability of a class by multiplying the probabilities of individual features.

- **Types of Naive Bayes Classifiers**:
  - **Multinomial Naive Bayes**: Suitable for discrete features (e.g., word counts in text).
  - **Bernoulli Naive Bayes**: Suitable for binary/boolean features (e.g., presence or absence of words).
  - **Gaussian Naive Bayes**: Suitable for continuous features.

### Why Naive Bayes?

- **Efficiency**: Naive Bayes models are computationally efficient and require less training time compared to more complex models.
- **Scalability**: The algorithm can handle large datasets effectively.
- **Performance**: Despite the naive assumption of feature independence, Naive Bayes often performs well in practice, especially for text classification tasks.

In this project, we use the Multinomial Naive Bayes classifier, which is particularly well-suited for text data where the features are word counts or frequencies.

## Project Structure

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

## Getting Started

1. **Setup**: Ensure all dependencies are installed by running `pip install -r requirements.txt`.
2. **Run the Workflow**: Execute `python Engine.py` to train the model.
3. **Make Predictions**: Use `python predict.py --test_complaint "your complaint text here"` to get predictions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


