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
