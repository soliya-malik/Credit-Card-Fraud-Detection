# Credit Card Fraud Detection

This repository contains a complete workflow for detecting fraudulent credit card transactions using machine learning techniques. The project leverages real-world transaction data and addresses the significant class imbalance inherent in fraud detection tasks.

# Dataset
The dataset used is creditcard.csv, which contains anonymized features (V1 to V28), Amount, Time, and a Class label (0: normal, 1: fraud).

# Project Workflow

# 1. Data Loading and Exploration

Loads the dataset with pandas and inspects its structure and basic statistics.

Checks for missing values and duplicate records.

# 2. Data Preprocessing

Scales the Amount feature using StandardScaler.

Drops the Time column as it is not informative for fraud detection.

Removes duplicate entries to ensure data quality.

# 3. Handling Class Imbalance

Undersampling: Balances the dataset by randomly sampling the majority class to match the minority (fraud) class.

Oversampling: Uses SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic samples for the minority class, resulting in a balanced dataset.

# 4. Model Training and Evaluation

Splits the data into training and testing sets.

# Trains multiple classifiers including:

Logistic Regression

Decision Tree Classifier

Evaluates models using accuracy, precision, recall, and F1-score to ensure robust fraud detection.

# 5. Model Persistence

The best-performing model (Decision Tree Classifier) is saved using joblib for future predictions.

# 6. Prediction Example

Demonstrates how to load the saved model and make predictions on new transaction data.

# How to Run

Install Dependencies

Prepare Data

Place creditcard.csv in the project directory.

Run the Notebook

Open and execute Credit-Card-Fraud-Detection.ipynb step by step.

# Model Inference

Use the provided code snippet to load the trained model and predict on new data.

# Key Features

End-to-end workflow: From data loading to model deployment.

Imbalance handling: Both undersampling and SMOTE oversampling approaches.

Multiple model comparison: Logistic Regression and Decision Tree.

# Model saving/loading: Easily persist and reuse trained models.

# Example: Predicting a Transaction

![WhatsApp Image 2025-04-25 at 21 57 18_5f063aef](https://github.com/user-attachments/assets/b22aa4be-09bd-4230-b1b3-612835c60853)

