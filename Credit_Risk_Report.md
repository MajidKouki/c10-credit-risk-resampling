# Credit Risk Resampling Report

## Overview of the Analysis:

The purpose of this analysis is to identify whether or not resampling, specifically oversampling, is an effective method of increasing a Logistic Regression model's accuracy and other evaluation statistics. The financial data used was historical lending data from a peer-to-peer lending company and the purpose was to identify healthy loans and risky loans. The process began by preparing the data before creating the model, fitting the model to the data, running predictions, and finally evaluating it's performance. After this, the data was oversampled in order to balance the classes before the same steps as before were taken with the intention of comparing both sets of results to identify if oversampling was able to increase the accuracy and other evaluation statistics of the model.

## Results:

0 - Healthy Loan
1 - Risky Loan

Machine Learning Model 1 (Standard Data):
* Balanced Accuracy Score - 0.9520479254722232 or 0.95
* Precision Score (0, 1, and Total) - 1.00, 0.85, and 0.99
* Recall Score (0, 1, and Total) - 0.99, 0.91, 0.99
* F1 Score (0, 1, and Total) - 1.00, 0.88, 0.99

Machine Learning Model 2 (Oversampled Data):
* Balanced Accuracy Score - 0.9936781215845847 or 0.99
* Precision Score (0, 1, and Total) - 1.00, 0.84, 0.99
* Recall Score (0, 1, and Total) - 0.99, 0.99, 0.99
* F1 Score (0, 1, and Total) - 1.00, 0.91, 0.99

## Summary

In summary, by comparing the performance of the two models, it can be seen that the model using oversampled data outperformed the standard model in nearly every measured statistic. While the oversampled model dropped 0.01 points in precision score (1), it made up with a 0.08 increase in recall score (1), a 0.03 increase in f1 score (1) and an increase of 0.04 in the balanced accuracy score. Although these numbers seem small, they all point towards an increase in almost all statistics for the oversampled model, showing it was the clear winner in terms of performance. The oversampled model had the highest scores all around for averages/totals as well as balanced accuracy. Due to this, the oversampled model is advised in any cases where a Logistic Regression model is needed for this data type.