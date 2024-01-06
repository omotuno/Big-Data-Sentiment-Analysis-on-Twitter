# Black Friday Tweets Sentiment Analysis Big Project

Sentiment analysis, also known as opinion mining, is a natural language processing approach that identifies the emotional tone behind a body of text.

## Project Overview

This project focuses on sentiment analysis of tweets related to Black Friday shopping events. The dataset is obtained from the Twitter API, stored in CSV format, and loaded into an Amazon S3 bucket via Amazon Kinesis Data Firehose. A machine learning pipeline is established to train a Logistic Regression model for supervised sentiment analysis. The model's accuracy is then calculated, and the prediction data is written to a personal S3 bucket for further analysis.

## Dataset

The dataset used is obtained from the Twitter API, containing tweets related to Black Friday shopping events. It is stored in CSV format, facilitating easy ingestion and storage through Amazon Kinesis Data Firehose.

## Machine Learning Pipeline

The machine learning pipeline comprises the following steps:

1. **Data Preprocessing:**
   - Removal of irrelevant information (URLs, special characters, emojis).
   - Text normalization techniques, including tokenization, stopword removal, and stemming/lemmatization.

2. **Feature Extraction:**
   - Transformation of cleaned text data into numerical features using techniques like bag-of-words or TF-IDF vectorization.

3. **Model Training:**
   - Training of a Logistic Regression model using labeled data with sentiment labels (positive, negative, or neutral).

4. **Model Evaluation:**
   - Calculation of accuracy, precision, recall, and F1-score to assess the model's performance.

5. **Prediction:**
   - Utilization of the trained model to predict sentiment for new, unseen tweets related to Black Friday.
   - Writing prediction results to a personal S3 bucket.

## Prerequisites

To run this project, you need:

- Access to Twitter API to obtain the dataset.
- An Amazon EC2 Instance for project deployment.
- An Amazon S3 bucket for storing the dataset and prediction results.
- Knowledge of machine learning techniques, particularly Logistic Regression.
- Python programming skills for implementing the machine learning pipeline.

## Usage

To use this project:

1. Obtain the Black Friday tweet dataset in CSV format using the Twitter API.
2. Load the dataset into an Amazon S3 bucket using Amazon Kinesis Data Firehose.
3. Preprocess the dataset by cleaning the text data and transforming it into numerical features.
4. Train a Logistic Regression model using the preprocessed data.
5. Evaluate the accuracy of the trained model using appropriate metrics.
6. Use the trained model to predict sentiment for new Black Friday tweets.
7. Write the prediction results to a personal S3 bucket for further analysis or visualization.

## Acknowledgment

This project is inspired by Weclouddata big data course, demonstrating sentiment analysis on tweets using Apache Spark on Databricks.

Feel free to customize the README further based on your preferences and additional project details!
