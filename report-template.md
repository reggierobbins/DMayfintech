# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
  -The purpose of the analysis was to create a model that would predict healthy loans and high risk loans using historical data.
  
* Explain what financial information the data was on, and what you needed to predict.
  -The data had financial information from previous loans. Including their loan size, interest rate, income, debt to income, and classification of the loan(healthy/high-risk).  Taking these features into account a model was created to predict healthy loans and high-risk loans.
   
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
 -The variables I was trying to predict with the model were healthy loans and high risk loans using the features of the loan.  

* Describe the stages of the machine learning process you went through as part of this analysis.
-I took the historical loan data and seperated the target(loan status) from the features of the loan.
-This allowed me to use a Support Vector Machine(SVM) for classification and regression analysis.  
-The (SVM) uses the loan features to train, test, and evaluate the loan.  Using these classifications and features allows the model to predict future credit risk based on the features.
  
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
-I used Logistic Regression to train the model on the features of healthy loans and high risk loans.
-I also used an oversampling method since the data included a majority of healthy loans.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
        *Model 1 Accuracy= 99.2%
        *Precision= 100% Healthy Loans and 85% High-Risk
        *Recall= 99% Healthy Loans, 91% High-Risk

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
        *Model 2 Accuracy= 99.4%
        *Precision= 100% Healthy Loans and 84% High-Risk
        *Recall= 99% for each
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
  - Machine Learning Model 2, because of its higher recall for both classifications.  The higher recall correlates to more comprehensive output and lower false negative rate.
    
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
-Perfomance does depend on the problem we are trying to solve. If it is more important to predict the 1's you would go with Model 1 because that model contains more healthy loan data with same Precision and Recall metrics.  And Model 2 for predicting the 0's because it has more "High-Risk" loan data and a better recall score with Precision minimally affected.
If you do not recommend any of the models, please justify your reasoning.
