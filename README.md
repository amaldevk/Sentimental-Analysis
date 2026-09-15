# Emotion Classification Using Machine Learning

## About the Project

This project focuses on classifying text comments into different emotion categories using Machine Learning.

The models used in this project are:

- Naive Bayes
- Support Vector Machine (SVM)

TF-IDF is used to convert text into numerical features before training the models.

## Dataset

The dataset contains **5,937 text comments** with two columns:

- `Comment` - The text given as input
- `Emotion` - The emotion label

The dataset contains three emotion categories:

- Anger
- Fear
- Joy

The dataset does not contain any missing values.

## Project Workflow

The project follows these steps:

1. Load the dataset
2. Explore the data
3. Check missing values
4. Preprocess the text
5. Split the dataset into training and testing data
6. Convert text into numerical features using TF-IDF
7. Train Naive Bayes model
8. Train Support Vector Machine model
9. Evaluate both models
10. Compare the model performance

## Text Preprocessing

The following preprocessing techniques were used:

- Convert text to lowercase
- Remove punctuation and special characters
- Tokenize the text into words
- Remove English stopwords

These steps help remove unnecessary text and allow the models to focus on more meaningful words.

## Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) was used for feature extraction.

TF-IDF converts text into numerical values that machine learning models can understand.

The final training data contained **4,749 samples and 7,733 TF-IDF features**.

## Machine Learning Models

### 1. Naive Bayes

Multinomial Naive Bayes was used as the first classification model.

### 2. Support Vector Machine

A linear Support Vector Machine was used as the second classification model.

SVM is suitable for text classification because it can work effectively with a large number of TF-IDF features.

## Results

| Model | Accuracy | Macro F1-Score |
|---|---:|---:|
| Naive Bayes | 89.06% | 89.05% |
| Support Vector Machine | 93.69% | 93.67% |

## Best Model

The **Support Vector Machine performed better** than Naive Bayes.

SVM achieved:

- **Accuracy: 93.69%**
- **Macro F1-Score: 93.67%**

Therefore, SVM was selected as the better model for this emotion classification task.

## Technologies Used

- Python
- Pandas
- NLTK
- Scikit-learn
- Google Colab

## Files

```text
Sentiment_Analysis.ipynb
nlp_dataset.csv
README.md
