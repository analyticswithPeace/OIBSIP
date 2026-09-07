# Twitter US Airline Sentiment Analysis

## Project Overview

This project focuses on analyzing the sentiment of tweets about US airlines and classifying them into three categories: **Negative, Neutral, and Positive**.

The project was completed as part of my data analytics learning journey with **Oasis Infobyte**.

## Objectives

- Explore and understand the airline sentiment dataset
- Clean and preprocess tweet text
- Convert text into numerical features using TF-IDF
- Build machine learning models for sentiment classification
- Evaluate and compare model performance
- Visualize sentiment patterns
- Identify and examine misclassified tweets

## Tools and Technologies

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- WordCloud
- Jupyter Notebook

## Project Workflow

1. Data Loading
2. Data Exploration
3. Text Cleaning and Preprocessing
4. TF-IDF Feature Extraction
5. Train-Test Split
6. Naive Bayes Model
7. Logistic Regression Model
8. Model Evaluation
9. Confusion Matrix Analysis
10. Sentiment Visualization
11. Word Cloud Visualization
12. Misclassified Tweet Analysis
13. Model Comparison

## Models Used

### Naive Bayes

Multinomial Naive Bayes was used as one of the classification algorithms for predicting the sentiment of airline tweets.

**Accuracy: 72.44%**

### Logistic Regression

Logistic Regression was used as the second classification algorithm.

**Accuracy: 76.37%**

Logistic Regression performed better overall than Naive Bayes on the test dataset.

## Model Comparison

| Model | Accuracy |
|---|---:|
| Naive Bayes | 72.44% |
| Logistic Regression | 76.37% |

## Visualizations

The project includes:

- Airline sentiment distribution
- Naive Bayes confusion matrix
- Logistic Regression confusion matrix
- Negative sentiment Word Cloud
- Neutral sentiment Word Cloud
- Positive sentiment Word Cloud

## Key Findings

The dataset contained more **negative tweets** than neutral or positive tweets.

Both models performed best when identifying negative tweets. However, neutral tweets were more challenging to classify correctly.

Logistic Regression achieved the highest accuracy of **76.37%**, making it the better-performing model between the two models tested.

## Conclusion

This project provided practical experience in **Natural Language Processing (NLP), text preprocessing, TF-IDF feature extraction, machine learning classification, model evaluation, and data visualization**.

The results demonstrate how machine learning can be applied to social media data to identify and classify customer sentiment.

## Author

**Peace Adeleke**

Data Analyst | Public Health Professional

## Acknowledgement

This project was completed as part of my learning experience with **Oasis Infobyte**.