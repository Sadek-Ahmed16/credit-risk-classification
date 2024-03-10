# credit-risk-classification
## Module 20 - Supervised learning - Credit Risk Classification

### Challenge Content

This repository includes the following files needed to to predict the loan status of a borrower; included for this challenge:

- 'Credit_Risk/Resources/lending_data.csv' (data)
- 'Credit_Risk/credit_risk_classification.ipynb' (notebook)
- 'Credit_Risk/report.md' (report)


## Overview

Using a dataset of historical lending activity from a peer-to-peer lending services company ('lending_data.csv'), a model bas been built to identify the creditworthiness of borrowers.

The analysis was based on evaluation of the Supervised Machine Learning Model 'LogisticRegression' to predict if a borrower's loan status is Healthy (0) or if the loan has a high risk of defaulting (1). The predictions were made againts the variables, loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks and total debt.

Stages of the Machine Learning Process:

- Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
- Split the data into training and testing datasets by using 'train_test_split'.
- Fit a logistic regression model by using the training data ('X_train' and 'y_train').
- Save the predictions on the testing data labels by using the testing feature data ('X_test') and the fitted model.
- Evaluate the model’s performance by Generating a confusion matrix, printing accuract score and classification report.
