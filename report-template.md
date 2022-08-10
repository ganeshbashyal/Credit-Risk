## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

## Credit Risk

Effective portfolio management does not only focus on distribution of funds but also identifying the type of risks and mitigate or eliminate. For a Bank the risk of credit risk is default on a debt by the borrower due to failed payments. The goal of Credit Risk identification and mitigation is to maximise the risk adjusted rate of return by maintaining credit risk exposure within acceptable parameters.

The proportion of healthy loans are a lot higher than the number of risky loans. Thus, the problem itself poses a classification problem that is inherently imbalanced.




## Analysing Data using Pyhton

In this analysis, Python will be used to perform machine learning in a credit data analysis. Initially data is imported to python from the lending_data.csv file provided. To clean up the data and have the structure ready, data is split into label sets(y) and features(X). The values of 0 in label sets implies that the loan is healthy and the value of 1 means that the loan has a higher risk of defaulting. 

The data is then split into training and testing data using train test split. A logistic Regression mode is then created with the original data. The data is then then resampled and another prediction is made through logistic regression this helps with the mitigation of the imbalance within the dataset. Since this problem is an imbalanced problem, several methods need to be explored thus, a confusion matrix and classification report is generated based on both models and comparison is made on the findings to determine the best model to use.


## Results

The results form machine learning on the original data Model 1 and on the oversampled data on Model 2 are as follows:

* Machine Learning Model 1:

  * Accuracy                            95.20%
  * Precision (Healthy Loan)            100%
  * Precision (High Risk Loan)          85%
  * Recall (Healthy Loan)               99%
  * Recall (High Risk Loan)             91%



* Machine Learning Model 2:
* 
    * Accuracy                            95.20%
    * Precision (Healthy Loan)            100%
    * Precision (High Risk Loan)          85%
    * Recall (Healthy Loan)               99%
    * Recall (High Risk Loan)             91%


## Summary

Since both models have similar accuracy it is challenging to choose the model to use but since we know that the precision is more important than recall on the high risk loan; the model with over sampled data is recommended. 
