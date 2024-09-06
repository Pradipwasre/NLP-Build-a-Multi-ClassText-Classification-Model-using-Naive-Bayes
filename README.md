## Modular Code Structure of the Project
Option 1: Tree-like Structure with Descriptions

## Folder Structure

- **Modular_code/**
  - Contains the main project files and directories.
  - **Input/**
    - `complaints.csv` — CSV file containing consumer complaints.
  - **Output/**
    - `count_vect.pkl` — Pickled CountVectorizer model.
    - `nb.pkl` — Pickled Naive Bayes model.
  - **Source/**
    - `model.py` — Script for training the Naive Bayes model.
    - `processing.py` — Functions for data preprocessing (tokenization, stopwords removal, etc.).
    - `utils.py` — Utility functions and helper methods.
  - `config.py` — Configuration file with file paths and global variables.
  - `Engine.py` — Main engine that runs the project workflow.
  - `naive_bayes.ipynb` — Jupyter notebook for experimentation and interactive development.
  - `predict.py` — Script for making predictions on new data using the trained model.
  - `README.md` — Documentation file for the project.
  - `requirements.txt` — List of required Python libraries for the project.
  - **nltk_data/**
    - Contains NLTK data such as stopwords for NLP processing.


---------------------------------------------------------------
Option 2: List Format with Bullet Points

## Folder Structure

- **Modular_code/**
  - Main project directory.
  - **Input/** — Contains input data:
    - `complaints.csv` — Dataset of consumer complaints.
  - **Output/** — Contains model output files:
    - `count_vect.pkl` — Serialized CountVectorizer for text vectorization.
    - `nb.pkl` — Serialized Naive Bayes model for classification.
  - **Source/** — Contains core Python scripts:
    - `model.py` — Model training script.
    - `processing.py` — Preprocessing functions (e.g., tokenization, cleaning).
    - `utils.py` — Utility functions and helpers.
  - `config.py` — Configuration settings (paths, parameters).
  - `Engine.py` — Main engine to run the model and processing pipeline.
  - `naive_bayes.ipynb` — Jupyter notebook for exploratory data analysis and code testing.
  - `predict.py` — Script to predict categories for new text inputs.
  - `README.md` — Project documentation.
  - `requirements.txt` — Python dependencies for the project.
  - **nltk_data/** — Data files for NLTK (e.g., stopwords).

---------------------------------------------------------------
Option 3: Heading and Sub-heading Style

## Project Directory

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
Option 4: Numbered Hierarchical Format

## Folder Structure

1. **Modular_code/**
   1.1 **Input/** — Contains input data file:
       - `complaints.csv` — The dataset of consumer complaints.
   1.2 **Output/** — Contains output from training:
       - `count_vect.pkl` — Pickled CountVectorizer model.
       - `nb.pkl` — Pickled Naive Bayes model.
   1.3 **Source/** — Contains source scripts:
       - `model.py` — Code for training the Naive Bayes classifier.
       - `processing.py` — Functions for text preprocessing (tokenization, cleaning).
       - `utils.py` — Helper functions used in the project.
   1.4 **config.py** — Configuration file with project settings and paths.
   1.5 **Engine.py** — The engine to run the workflow.
   1.6 **naive_bayes.ipynb** — Jupyter notebook for exploratory data analysis.
   1.7 **predict.py** — Script for predicting categories for new text input.
   1.8 **README.md** — Project overview and documentation.
   1.9 **requirements.txt** — Python dependencies for the project.
   1.10 **nltk_data/** — NLTK resources (e.g., stopwords).

---------------------------------------------------------------
Option 5: Simple Bullet List with File Types


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
