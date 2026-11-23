# SMS Spam Classification using NLP

## Overview
This project implements an SMS Spam Classification system using Natural Language Processing (NLP) and Machine Learning. It classifies text messages into two categories:

- **Ham:** Legitimate messages.
- **Spam:** Unwanted or promotional messages.

The project explores text preprocessing, feature extraction, and multiple machine learning algorithms to identify spam messages.

## Technologies Used
- Python
- NumPy
- Pandas
- NLTK
- Scikit-learn

## Project Workflow

1. **Data Loading:** Import and explore the SMS Spam Collection dataset.
2. **Text Preprocessing:**
   - Convert text to lowercase.
   - Remove punctuation and extra whitespace.
   - Remove stopwords.
   - Apply Porter Stemming.
   - Replace numbers with a common token.
3. **Tokenization:** Split messages into individual words.
4. **Feature Extraction:** Build a Bag-of-Words representation using the 1,500 most common words.
5. **Model Training:** Train multiple machine learning classifiers.
6. **Evaluation:** Compare model performance using accuracy, precision, recall, F1-score, and a confusion matrix.

## Machine Learning Algorithms

The following classifiers were implemented:

- Support Vector Classifier (SVC)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Logistic Regression
- Voting Classifier

## Results

| Algorithm | Accuracy |
|---|---:|
| SVC | 98.42% |
| KNN | 95.33% |
| Decision Tree | 97.42% |
| Random Forest | 98.28% |
| Logistic Regression | 98.64% |
| Voting Classifier | 98.64% |

*Results are based on the notebook's reported execution outputs.*

## Dataset
The project uses the SMS Spam Collection dataset, containing SMS messages labelled as spam or ham.

## Installation

Clone the repository:


Install the required libraries:

```bash
pip install numpy pandas nltk scikit-learn
```

Download the required NLTK resources:

```python
import nltk

nltk.download('punkt')
nltk.download('stopwords')
```

## Run the Project

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebook cells sequentially to execute preprocessing, feature extraction, model training, and evaluation.

## Future Improvements
- Experiment with TF-IDF feature extraction.
- Explore advanced NLP techniques.
- Compare traditional ML models with deep learning approaches.
- Build an interactive interface for real-time SMS classification.
