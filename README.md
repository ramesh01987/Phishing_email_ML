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
* Data Preprocessing: Text data is vectorized using TF-IDF to convert it into numerical format suitable for SVM.
* Handling Imbalance: The dataset is imbalanced, so we use RandomUnderSampler to balance the classes.
* Model Training: SVM model is trained using the balanced data.
* Evaluation: Model performance metrics such as accuracy, precision, recall, and F1-score are calculated and visualized using     confusion matrix and PR curve.
* Cross-Validation: estimate of how well SVM model will generalize to new data
* Grid Search : identify the optimal combination of hyperparameters for a machine learning model

## Real-World Test
To evaluate the SVM model's classification performance in a real-world scenario, I conducted tests using emails extracted from my personal Gmail account. This test aimed to assess how effectively the model can distinguish between phishing and non-phishing emails based on real, diverse email data.

## Comparing Models: Random Forest vs. Linear Regression
To explore alternative modeling approaches, I experimented with both Random Forest and Linear Regression classifiers on the dataset. The goal was to determine if either model could offer superior performance metrics compared to the SVM model previously discussed.

## Results
After evaluating multiple classifiers on the dataset of phishing and non-phishing emails, the following results were obtained:

* (SVM) Accuracy: 97% , Cross-Validation Accuracy: 88.00% +/- 10.00 %

* Logistic Regression Accuracy: 96%, Cross-Validation Accuracy: 97.00% +/- 0.00%

* Random Forest Accuracy: 98%, Cross-Validation Accuracy: 98.00% +/- 0.00%




  
