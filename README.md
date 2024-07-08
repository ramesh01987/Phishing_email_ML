# Overview

This project aims to build a model that can effectively distinguish between phishing and non-phishing emails using machine learning techniques. We utilize a dataset containing various email sources, obtained from Kaggle :https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset

## Dataset Exploration

The dataset includes multiple CSV files, each representing different email datasets. Here's a summary of the datasets used:

- **SpamAssasin.csv**
- **Nigerian_Fraud.csv**
- **phishing_email.csv**
- **CEAS_08.csv**
- **Enron.csv**
- **Ling.csv**
- **Nazario.csv**

In our case we are going to focus on phishing_email.csv

## Model Building 

Given the dataset's characteristics, we opt for a supervised learning approach using Support Vector Machines (SVM).

Steps:

    Data Preprocessing: Text data is vectorized using TF-IDF to convert it into numerical format suitable for SVM.

    Handling Imbalance: The dataset is imbalanced, so we use RandomUnderSampler to balance the classes.

    Model Training: SVM model is trained using the balanced data.

    Evaluation: Model performance metrics such as accuracy, precision, recall, and F1-score are calculated and visualized using confusion matrix and PR curve.

    Saving the Model: The trained SVM model is saved for future use.
