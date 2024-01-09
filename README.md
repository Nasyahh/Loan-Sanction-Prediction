# Bank Loan Sanction Prediction

## Overview
This project aims to *predict the bank loan sanction amount* for each loan applicant based on their personal and financial information. The project uses a *tuned random forest model, which is an ensemble learning technique that combines multiple decision trees to produce a more accurate and robust prediction. The model is evaluated using the **mean absolute percentage error (MAPE)*, which is a measure of how close the predictions are to the actual values.

## Data
The data consists of *30,000* loan applicants with *24* features, such as name, income, occupation, credit score, loan amount, default, etc. The target variable is the *loan sanction amount*, which is the amount of money that the bank approves to lend to the applicant. The data is obtained from [Kaggle](^1^).

## Method
The method used for this project is as follows:

- First, the data is *explored* and *preprocessed* by performing descriptive statistics, handling missing values, encoding categorical variables.
- Second, the data is *split* into training and testing sets with a ratio of 80:20.
- Third, a *random forest model* is *trained* on the training set using the default hyperparameters.
- Fourth, the model is *tuned* using *grid search* and *cross-validation* to find the optimal hyperparameters, such as the number of trees, the maximum depth, the minimum samples split, etc.
- Fifth, the model is *tested* on the testing set and the *MAPE* is calculated to evaluate the model performance.

## Result
The result of the project is as follows:

- The tuned random forest model achieved a MAPE of *4%*, which means that the average error of the predictions is 4% of the actual loan sanction amount. This indicates that the model is able to predict the loan sanction amount with a high degree of accuracy.
- The model also showed a good *feature importance* ranking, which reveals the most influential features for the prediction. The top three features are: loan amount, income, and credit score.
