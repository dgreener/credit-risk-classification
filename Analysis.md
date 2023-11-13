# Credit Risk Model

## Overview of the Analysis

I used historical lending data from a peer-to-peer lending services company to build a predictive model for assessing the credit risk of borrowers.

The model utilized the following financial data as independent variables: loan size, interest rate, borrower income, derogatory marks, debt to income ratio, number of accounts. These were used to predict "loan status", which is a measure of loan risk.

We can see a discrepancy in the outcome measure - "loan status" - with there being a count of 75,036 low-risk loans vs. 2,500 high-risk loans. 

The following were steps I used in my analysis: data pre-processing, training, and evaluation of model.


## Results


* Machine Learning Model 1:
  * Accuracy: The balanced accuracy was 95.2%.
  * Precision: The precision for detecting low-risk loans was 100% vs. 85% for high-risk loans.
  * Recall scores: The recall scores were 0.99 and 0.91 for low- and high-risk loans, respectively.



* Machine Learning Model 2:
  * Accuracy: The balanced accuracy was 99.4%.
  * Precision: The precision for detecting low-risk loans was 100% vs. 84% for high-risk loans.
  * Recall scores: The recall scores were 1.00 and 0.91 for low- and high-risk loans, respectively.

## Summary

Machine Learning Model 2 seems to perform slightly better than Machine Learning Model 1, on the basis of having higher test accuracy with eqvuialent precision and recall scores. The reason why Model 2 performs better is because it randomly oversamples high-risk loan data. In Model 1, high-risk loans only account for 2.6% of all loans, meaning that any statistical correlation with the independent variables may be skewed (either positively or negatively). 

For a bank, there are distinct risks for falsely labeling a low-risk loan applicant as "high risk" and vice versa. In the event a bank fails to identify a high-risk loan, it stand a higher chance of a loan default. Conversely, if the bank fails to identify a low-risk loan, then it stands to lose business. In this scenario, it is imperative that the model accurately predict both high-risk (1) and low-risk (0) loans.

