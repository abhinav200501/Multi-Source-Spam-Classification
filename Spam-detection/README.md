# Multi-Source Spam Classification

## Overview

This project develops a machine learning system to classify text messages as **Spam** or **Ham (legitimate)**. The project combines multiple text sources, including SMS and email/HTML data, into a unified dataset and applies natural language processing and machine learning techniques for classification.

The objective is to build a robust classifier that can handle spam detection across different message formats.

## Problem Statement

Spam messages are commonly found in SMS, emails, and other text-based communication platforms. Because spam messages can vary significantly in structure and wording, a classification model needs to process and learn from diverse text sources.

This project uses Natural Language Processing (NLP) techniques to transform raw text into machine-readable features and trains machine learning models to classify messages as spam or ham.

## Dataset & Data Processing

Multiple sources were combined to create a unified dataset containing SMS and email-based messages.

The preprocessing pipeline includes:

- Parsing raw email/HTML files
- Extracting text content from different message formats
- Combining multiple datasets
- Removing duplicate records
- Tokenization
- Stop-word removal
- Porter stemming
- Text normalization
- Feature extraction using TF-IDF / Count Vectorization

The resulting dataset was used to train and evaluate the classification models.

## Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **NLTK**
- **Scikit-Learn**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**
- **Git & GitHub**

## Machine Learning Models

The following classification algorithms were evaluated:

- Multinomial Naive Bayes
- Gaussian Naive Bayes
- Support Vector Classifier (SVC)

Hyperparameter optimization was performed using:

- GridSearchCV
- Cross-validation
- Model comparison

The final model achieved approximately **96% classification accuracy** on the evaluated dataset.

## Project Workflow

```text
Raw SMS / Email Data
        ↓
Data Collection & Parsing
        ↓
Data Cleaning
        ↓
Duplicate Removal
        ↓
Text Preprocessing
        ↓
Tokenization
        ↓
Stop-word Removal
        ↓
Stemming
        ↓
Feature Extraction
        ↓
Train/Test Split
        ↓
Model Training
        ↓
Hyperparameter Tuning
        ↓
Model Evaluation
        ↓
Spam / Ham Prediction
