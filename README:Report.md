# Module 20 Report: Credit Risk Classification

## Overview of the Analysis

The purpose of this analysis was to build a supervised machine learning model that can predict credit risk. The dataset included historical financial data from a peer-to-peer lending company, and the goal was to determine whether a loan is high risk (`1`) or healthy (`0`).

The `loan_status` column served as the target variable, where:
- `0` indicates a healthy loan
- `1` indicates a high-risk loan

The feature set included:
- `loan_size`
- `interest_rate`
- `borrower_income`
- `debt_to_income`
- `num_of_accounts`
- `derogatory_marks`
- `total_debt`

The machine learning process included:
- Importing and preprocessing the data
- Splitting the data into training and testing sets
- Training a logistic regression model
- Making predictions and evaluating the model using a confusion matrix and classification report

## Results

* **Machine Learning Model: Logistic Regression**
  * **Accuracy**: 99%
  * **Precision**:
    * Class 0 (healthy loans): 1.00
    * Class 1 (high-risk loans): 0.84
  * **Recall**:
    * Class 0: 0.99
    * Class 1: 0.94
  * **F1-Score**:
    * Class 0: 1.00
    * Class 1: 0.89

## Summary

The logistic regression model performs very well overall, with an accuracy of 99%. It predicts healthy loans with near-perfect precision and recall, and it also performs well in identifying high-risk loans, with a recall score of 94%. This suggests the model is effective at both minimizing false positives and catching true positives in high-risk loan cases.

Because predicting high-risk loans accurately is critical for the company to avoid defaults, this model is a strong candidate for use. I recommend implementing the logistic regression model as a baseline, while also considering additional models (e.g., random forest or boosting algorithms) for further performance evaluation and comparison.
