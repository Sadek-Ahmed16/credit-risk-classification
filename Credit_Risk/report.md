# Module 12 Report

## Overview of the Analysis

Using a dataset of historical lending activity from a peer-to-peer lending services company ('lending_data.csv'),  a model bas been built to identify the creditworthiness of borrowers.

The analysis was based on evaluation of the Supervised Machine Learning Model 'LogisticRegression' to predict if a borrower's loan status is Healthy (0) or if the loan has a high risk of defaulting (1). The predictions were made againts the variables, loan size, interest rate,  borrower income, debt to income ratio, number of accounts,	derogatory marks and	total debt.

Stages of the Machine Learning Process:
* Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
* Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
* Split the data into training and testing datasets by using 'train_test_split'.
*  Fit a logistic regression model by using the training data ('X_train' and 'y_train').
*  Save the predictions on the testing data labels by using the testing feature data ('X_test') and the fitted model.
*  Evaluate the model’s performance by Generating a confusion matrix, printing accuract score and classification report.


## Results

Machine Learning Model 'LogisticRegression':

   * For class 0 (healthy loan):
       Precision: 1.00 (100%)
       Recall: 1.00 (100%)
       F1-score: 1.00 (100%)
       Support: 18759

   These metrics indicate excellent performance for predicting healthy loans (class 0). The model rarely misclassifies healthy loans and captures nearly all of them.

   * For class 1 (high-risk loan):
       Precision: 0.87 (87%)
       Recall: 0.89 (89%)
       F1-score: 0.88 (88%)
       Support: 625

   The model performs well for high-risk loans (class 1) with slightly lower but still reasonable precision, recall, and F1-score. It correctly identifies a high percentage of high-risk loans (recall), and when it predicts a high-risk loan, it is correct most of the time (precision). The F1-score, which is the harmonic mean of precision and recall, remains high.



   * Accuracy Score: 0.9924164259182832 (99.24%)

   The overall accuracy of the model is 99%, indicating its effectiveness in making correct predictions for both classes.


## Summary

In summary, the logistic regression model is highly accurate for predicting healthy loans (class 0) and performs well for high-risk loans (class 1) with a slightly lower but still reasonable precision, recall, and F1-score. The overall accuracy of the model is 99%, for this reason, this Logical regression model is recomended to predict the loan status of a borrower for this company.




