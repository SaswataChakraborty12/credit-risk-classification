# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis is to create and evaluate the accuracy of a data model that predicts the credity worthiness of potential borrowers from peer-to-peer lending services.
 
The dataset contains financial attributes related to loan applicants, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

The goal is to use this information to predict and classify loans into two categories: Healthy Loans (Class 0) and High-Risk Loans (Class 1) based on their associated risk factors or repayment potential.

The analysis began by collecting lending data from a CSV file, followed by dividing it into features and the target variable ('loan_status'). The data was split into training and testing sets for model training and evaluation.

For the analysis, LogisticRegression method was used and was trained using the training dataset. Subsequently, predictions were made on the test data, and various metrics were computed to assess the model's performance. Additionally, the imbalanced-learn library's RandomOverSampler was implemented to tackle class imbalance. This technique addresses skewed class distributions, specifically in the context of high-risk loans, by generating synthetic samples to create a more balanced dataset for improved model training and performance in predicting high-risk loans accurately.

## Results

Machine Learning Model:

Balanced Accuracy Score: 0.97
Precision (Class 0 - Healthy Loan): 1.00
Recall (Class 0 - Healthy Loan): 0.99
Precision (Class 1 - High-Risk Loan): 0.84
Recall (Class 1 - High-Risk Loan): 0.94


## Summary

Model showcases exceptional performance in identifying healthy loans, maintaining high precision and recall. For high-risk loans, it displays a slightly lower precision but still maintains good recall. The balanced accuracy score indicates a strong overall ability to predict both classes.


Considering the importance of correctly identifying high-risk loans while minimizing false alarms (misclassifying healthy loans as high-risk), this Model is definitely suitable.

