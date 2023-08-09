# Module 12 Report

## Overview of the Analysis

This analysis has the purpose to find the best model to identify salable loans and high-risk loans.

The dataset shows details about loans made. The prediction should read the parameters and identify a loan as healthy, flagged here as loan_status 0, or risky loan flagged here as loan_status 0

|| loan_size | interest_rate | borrower_income | debt_to_income | num_of_accounts | derogatory_marks | total_debt | loan_status |
|-|-|-|-|-|-|-|-|-|
| 0 | 10700.0 | 7.672 | 52800 | 0.431818  | 5 | 1 | 22800 | 0 |
| 1	| 8400.0	| 6.692	| 43600	| 0.311927	| 3	| 0	| 13600	| 0 |
| 2	| 9000.0	| 6.963	| 46100	| 0.349241	| 3	| 0	| 16100	| 0 |
| 3	| 10700.0	| 7.664	| 52700	| 0.430740	| 5	| 1	| 22700	| 0 |
| 4	| 10800.0	| 7.698	| 53000	| 0.433962	| 5	| 1	| 23000	| 0 |
| 77531	| 19100.0	| 11.261	| 86600	| 0.653580	| 12	| 2	| 56600	| 1 |
| 77532	| 17700.0	| 10.662	| 80900	| 0.629172	| 11	| 2	| 50900	| 1 |
| 77533	| 17600.0	| 10.595	| 80300	| 0.626401	| 11	| 2	| 50300	| 1 |
| 77534	| 16300.0	| 10.068	| 75300	| 0.601594	| 10	| 2	| 45300	| 1 |
| 77535	| 15600.0	| 9.742	| 72300	| 0.585062	| 9	| 2	| 42300	| 1 |

In total at the data set, is identified: </br>
75036 healthy loans, flagged as 0 and </br>
2500 risk loans, flagged as 1 </br>

To differentiate healthy loans from risky loans. First, the data set is divided into training and testing.
After, the training data is used to train the model to identify the desired results. For this, the LogisticRegression function is used, which receives the training data and creates a return model, this model is used receiving the test data to generate a prediction.
With the prediction generated on top of the test data, we can assess the accuracy of the model and identify whether it can be used in a real environment.



## Results

Two analysis models were made based on the provided data set. Here are the results

* Machine Learning Model 1:
  * Accuracy 95.20%
  * Precision for healthy loans 100%
  * Precision for risky loans 85%
  * Recall for healthy loans 99%
  * Recall for risky loans 91%

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Accuracy 99.47%
  * Precision for healthy loans 99%
  * Precision for risky loans 99%
  * Recall for healthy loans 99%
  * Recall for risky loans 99%

## Summary

Both models achieved Accuracy results greater than 95% of Accuracy. However, despite model 1 being able to more effectively identify cases of healthy loans, it is more interesting that risky loans are the focus of the model, therefore, model 2 which achieved the highest Accuracy for risky loans is the most indicated to be used.