# Module 12 Report Template

## Overview of the Analysis

* The purpose of this analysis is to develop machine learning models for credit risk.
* The dataset contains financial information on loans, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status
* The variable we were trying to predict is "loan_status," and with the [value_counts()] function we see the distribution of healthy loans and high-risk loans in the dataset 
* Stages of the machine learning process:
Data Loading and Preprocessing
Data Splitting
Model Building
Model Evaluation

* Methods Used:
I used logistic regression, a commonly used classification algorithm, to build both models
I also utilized the RandomOverSampler method from the "imbalanced-learn" library to handle class imbalance in the dataset.

## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
* Balanced Accuracy Score: 0.85
* Precision and Recall Scores:
  * Precision for label 0 (healthy loan): 1.00
  * Precision for label 1 (high-risk loan): 0.79
  * Recall for label 0: 0.73
  * Recall for label 1: 1.00


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
* Balanced Accuracy Score: 0.75
* Precision and Recall Scores:
  * Precision for label 0: 0.78
  * Precision for label 1: 0.80
  * Recall for label 0: 0.81
  * Recall for label 1: 0.77

## Summary

Both models demonstrate reasonable performance in predicting credit risk. The original data logistic regression model achieves a higher balanced accuracy score (0.85) compared to the model trained with resampled data (0.75). However, the model with resampled data exhibits better recall for high-risk loans, indicating its effectiveness in identifying loans at risk of defaulting.And personally the original data logistic regression model could be favored despite its slightly lower recall for high-risk loans.
