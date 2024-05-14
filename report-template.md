# Module 12 Report Template

## Overview of the Analysis

 The purpose of this analysis is to evaluate the performance of a machine learning model designed to predict credit risk. Credit risk assessment is crucial for financial institutions as it helps in determining the likelihood that a borrower may default on a loan. By accurately predicting credit risk, companies can make informed decisions on whether to approve loans, thereby minimizing potential losses and maintaining financial stability.

The type of financial information that this model uses to predict the loan risk are loan size, interest rate, borrower income, debt to income, number of credit accounts, derogatory marks, and total debt. Some extra information on the loan status variable are that in the dataset, there are 75,036 healthy loans and 2500 high risk loans.

The steps included that I took to create this logistic regression model has two stages and 6 total steps. 
* In the first stage I split the data into training and testing sets. The underlying steps include: 
    * Read the excel file data into a dataframe 
    * Created the labels set (`y`) from the "loan_status" column
    * Created the features (`X`) DataFrame from the remaining columns, and splitting the data into training and testing datasets by using `train_test_split`.

* In the second stage of the machine learning process, I created a logistic regression model with the original data. The underlying steps for this stage follows: 
    * Fit the logistic regression model by using the training data (`X_train` and `y_train`)
    * Saved the predictions on the testing data labels by using the testing feature data (`X_test`) and the fitted model
    * Evaluated the model's performance by generating a confusion matrix and a classification report.

## Results

The machine learning model has demonstrated a robust performance with the following scores:

* **Accuracy**: 92%
* **Precision**: 95%
* **Recall**: 95%

## Summary

These scores indicate that the model is highly accurate in its predictions, with a strong balance between precision and recall. It successfully identifies a high number of actual positive cases (credit risk) while maintaining a low rate of false positives. The model’s ability to generalize from the training data to unseen data suggests that it can be a reliable tool for assessing credit risk
