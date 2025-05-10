#  Question Pair Similarity Classification

This project tackles the challenge of identifying whether two given questions are duplicates. Duplicate questions are common in large Q&A platforms like Quora, and detecting them is essential to improve user experience and avoid redundancy.

---

##  Objective

The goal is to build a machine learning model that classifies whether a pair of questions are semantically similar or not using the [Quora Question Pairs dataset](https://www.kaggle.com/competitions/quora-question-pairs).

---

##  Dataset

**Source**: Quora Question Pairs via Kaggle

### Features:
- `id`: Unique identifier for each row
- `qid1`, `qid2`: Unique IDs for the questions
- `question1`, `question2`: Text content of the two questions
- `is_duplicate`: Target label (1 = Duplicate, 0 = Not Duplicate)

---

##  Exploratory Data Analysis (EDA)

EDA was conducted to gain insights into the dataset, including:
- Class imbalance visualization
- Distribution of question lengths
- Frequency of duplicate vs non-duplicate pairs
- Word clouds of questions

_Key Observations_:
- The dataset has class imbalance: more non-duplicates than duplicates.
- Duplicate questions tend to be slightly shorter.

---

##  Text Preprocessing

To prepare the text for modeling, the following steps were applied:

- Lowercasing
- Removing punctuation and special characters
- Removing stopwords
- Lemmatization using NLTK’s WordNetLemmatizer
- Sentence normalization


##  Models Applied

### Classical Models:
- **Logistic Regression**


### Deep Learning Models:
- **Artificial Neural Network (ANN)** 
- **LSTM-based model** 

Model Evaluation

Models were evaluated using:

- Accuracy
- Precision, Recall, F1-score
- AUC-ROC
- Confusion Matrix

