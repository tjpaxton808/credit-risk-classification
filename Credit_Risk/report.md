# Module 20 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis was to assess credit risk using machine learning techniques. Specifically, we aimed to predict whether a loand is high-risk (1) or healthy (0) based on various financial features.

The dataset consusts of financial information related to loans, with loan_status service as the target variable.
To conduct the analysis, we followed these marchine learning steps:
* Loaded the dataset and performed preprocessing.
* Split the data into training and testing sets.
* Trained a Logistic Regression model to classify loan risk.
* Evaluated the model using accuracy, precision, recall, and an F1-score.
The Logistic Regression model was selected due to its efficiency in handling binary classification problems.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
* Accuracy: 99%
* Precision:
    * Healthy loans (0): 1.00 - Almost all predicted healthy loans were correct.
    * High-risk loans (1): 0.84 - 84% of predicted high-risk loans were truly high-risk.
* Recall:
    * Healthy loans (0): 0.99 - The model captured almost all of the actual healthy loans.
    * High-risk loans (1): 0.94 - The model correctly identified 94% of high-risk loans.


## Summary

The Logistic Regression model performed best based on its 99% accuracy and strong ability to distinguish between healthy and high-risk loans. It correctly identifies 94% of actual high-risk loans (recall = 0.94), making it effective at flagging risky loans. However, 16% of loans predicted as high-risk are actually healthy (precision = 0.84).

The importance of the model's performance depends on the business goal. If identifying all potential defaults is the priority, the high recall for Class 1 (0.94) makes this model useful. If avoiding false high-risk classifications is more important, the model may need improvement, as it sometimes mislabels healthy loans.

Recommendation: The model is suitable for identifying high-risk loans but should be refined if false positives are a concern.