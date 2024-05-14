# Module 12 Credit Risk Classification
![Alt text](Logo-1.webp)

## Overview of the Analysis
In this Challenge, I have used various techniques to train and evaluate a model based on loan risk. We have used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis is to create and evaluate the accuracy of a data model that predicts the credity worthiness of potential borrowers from peer-to-peer lending services
* Explain what financial information the data was on, and what you needed to predict.
We had the below financial information as variables as X variables
    Loan Size
    Intrest Rate
    Borrower Income
    Debt to income ratio
    number of accounts
    Number of derogatory remarks
    Total debt

    Our target variable was "Loan Status"

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
As part of the project we were trying to predict the value for loan status. A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting
* Describe the stages of the machine learning process you went through as part of this analysis.
As part of the machine learning analysis, we have performed the below steps
   Reading the data and converting to a data frame.
   Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns
   Split the Data into Training and Testing Sets by using train_test_split.
   Creating a Logistic Regression Model with the Original Data
      Fit a logistic regression model by using the training data (X_train and y_train).
      Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model.
      Evaluate the model’s performance



* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
In this project we used LogisticRegression model to predict the loan status. Logistic regression estimates the probability of an event occurring,  based on a given data set of independent variables.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
![Alt text](Accurecy-1.png)

Precision Score: 92% --> This means 92% of predicted positives were correct
Recall Score: 95% --> this means that the model was 95% precise in measuring true positive values our of all positive predictions made



## Summary

I would recommend using this model to predict the creditworthiness of borrowers, because it has over 95% accuracy in predicting the outcome of the repayment of the initial loan. That accuracy range could be easily molded into a business risk profile to ensure sufficient capital flow for the lenders to remain in business/make a profit.