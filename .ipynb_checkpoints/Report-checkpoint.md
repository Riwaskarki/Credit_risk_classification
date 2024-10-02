# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to develop a machine learning model that can predict whether a loan is healthy (low risk) or high-risk based on key financial information. This helps financial institutions assess the risk associated with lending to borrowers.

## Machine Learning Process:
Feature Selection: The features (loan_amnt, int_rate, annual_inc, total debt etc) were selected to train the model. The target label was the loan status.

Data Splitting: The data was split into training and testing sets using train_test_split to ensure the model could be trained on one portion of the data and evaluated on another.

Model Selection: The Logistic Regression algorithm was chosen for this binary classification problem. Logistic Regression is a commonly used supervised learning method, particularly for predicting binary outcomes (healthy or high-risk loan in this case).

Model Training: The model was trained on the training dataset to learn the patterns that differentiate healthy loans from high-risk loans.

Evaluation: After training, the model was evaluated on the testing dataset using metrics such as:

Confusion matrix: To visualize the correct and incorrect predictions for both loan statuses.
Classification report: To provide precision, recall, and F1-scores for the model's performance on healthy and high-risk loans.
Methods Used:
Logistic Regression: This algorithm was used to predict the probability of a loan being either healthy or high-risk, based on the financial features provided.

## Results
* Healthy Loans (0): Precision, recall, and F1-score are all perfect at 1.00, indicating flawless prediction of healthy loans.
* High-Risk Loans (1): The model has 0.86 precision, 0.91 recall, and an F1-score of 0.88, meaning it predicts most high-risk loans correctly but has some misclassifications.
* Overall Accuracy: The model achieves a high accuracy of 99%, performing very well across both categories, especially for healthy loans.


## Summary

The overall accuracy of the model was 99%, suggesting that it is highly reliable, especially given the dataset's imbalance, where healthy loans are more frequent
I recommend using this Logistic Regression model for predicting loan status. It has excellent performance for healthy loans and strong performance for high-risk loans. However, if the goal is to minimize the number of false negatives (missed high-risk loans), further tuning or using additional models (like Random Forest or Gradient Boosting) could improve performance on high-risk loans.
