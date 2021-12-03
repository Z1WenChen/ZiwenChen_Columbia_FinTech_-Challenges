# Module 12 Report Template

## Overview of the Analysis

* The purpose of this analysis is to use Machine Learning models to fit and predict the loan status of the data with different features, such as "loan size" and "interest rate". We denote "0" as healthy loan which is probably not default , and "1" as high-risk loan which is likely to default.

* The financial data consists of 7 features: "loan_size", "interest_rate", "borrower_income", "debt_to_income", "number_of_accounts", "derogatory_marks", and "total_debt". We need to predict whether the loan is healthy or not (loan status is "0" or "1").

* From the value_counts method, we can observe that there are 75036 health loans and 2500 high-risk loans from the dataset. And, we want to predict the loan status is healthy or high-risk.

* We are predicting through a Logistic Regression Model with the original data and predicting through a Logistic Regression Model with Resampled Training Data. We split the data into train and test data, fit the train data, and predict through the model. Then we can choose the better model through comparing the accuracy, precision, recall, and F1 score from confusion matrix and classification report.

* We use `LogisticRegression`, and `LogisticRegression` with oversampling method as two models.



## Results

* Machine Learning Model 1: logistic regression model
  * Description of Model 1 Accuracy: 0.9918, Precision: 0.9945, and Recall scores: 0.9970.



* Machine Learning Model 2: logistic regression model with oversampling method
  * Description of Model 2 Accuracy: 0.9938, Precision: 0.9938, and Recall scores: 0.9997.


## Summary

* The logistic regression model fitted with the oversampled data predicts very well on both healthy and high-risk loan labels. We can observe from the classification report that the precision for "0" is 100% and the precision for "1" is 84%. The recall is also pretty good for "0" as 99% is correct, and "1" as 99% correct. F1-score is also high for both healthy and high-risk loan, which demonstrates that the model performs well. All of these results are higher than those of the logistic regression model fitted with test data, expect the precision on "1".

* Comparing with the logistic regression model fitted with test data, the logistic regression model fitted with oversampled data predicts better. From the prints above, we can find that the model with oversampled data performs better than the model fitted with test data by a higher correctness in recall (0.9997 > 0.9970) and Accuracy (0.9938 > 0.9918). Even though the model fitted with oversampled data underperforms slightly on precision (0.9938 < 0.9945) than the model fitted with test data, the model fitted with oversampled data still overall outperforms than the model fitted with test data.

* Since we are more interested in the prediction on "1" (high-risk loan with label) for risk-management, the logistic regression model fitted with oversampled data probably is a better choice.
