# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

For this project, the purpose was to conduct a comprehensive analysis using machine learning modules to predict the loan status based on historical lending data. Going through the module, I implemented modules that could predict whether a loan will be healthy or non- healthy, using various financial features. 


* Explain what financial information the data was on, and what you needed to predict.

The dataset used for this analysis contains financial information about loans, including variables such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. 

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The target variable to be predicted is the loan_status, where 0 indicates a healthy loan and 1 indicates a high-risk loan.

* Describe the stages of the machine learning process you went through as part of this analysis.

1.) Data Loading and Preprocessing: Loaded the dataset into a Pandas DataFrame and separated the features (X) from the target variable (y).
2.) Data Splitting: Split the data into training and testing sets using train_test_split from sklearn.
3.) Model Training: Trained a Logistic Regression model using the training data.
4.) Prediction and Evaluation: Made predictions on the test data and evaluated the model's performance using accuracy, precision, recall, and F1-score metrics.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
Logistic Regression: A statistical method for binary classification which was used to predict the probability of a loan being healthy or high-risk.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
Logistic Regression
Accuracy: 99%
Precision:
Healthy Loans (0): 1.00
High-Risk Loans (1): 0.85
Recall:
Healthy Loans (0): 0.99
High-Risk Loans (1): 0.91
F1-Score:
Healthy Loans (0): 1.00
High-Risk Loans (1): 0.88
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?

Based on the performance metrics, the Logistic Regression model is highly recommended for predicting loan statuses. The model's high accuracy and balanced precision and recall scores make it suitable for identifying both healthy and high-risk loans effectively.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The importance of predicting healthy versus high-risk loans depends on the context and the cost associated with misclassification:
- High Recall for High-Risk Loans (1): Critical in minimizing financial losses by ensuring most high-risk loans are correctly identified.
- High Precision for Healthy Loans (0): Important to avoid falsely classifying healthy loans as high-risk, which could lead to unnecessary rejection of loans.


If you do not recommend any of the models, please justify your reasoning.

Given the performance metrics and the context of the data, I would recommend that there be more exploration and tuning of models. This might improve the predictive performance for high-risk loans, ensuring a more balanced and effective model. This approach would help in achieving higher recall and precision scores for high-risk loans, thus better serving the needs of a lending company in mitigating financial risks.

