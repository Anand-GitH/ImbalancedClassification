# ImbalancedClassification
Credit Card Fraud Detection - Imbalanced Dataset Classification using Near Miss and SMOTE techniques

https://www.kaggle.com/mlg-ulb/creditcardfraud

The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

Such datasets will have class imbalance so any classifier if classifies all observations as majority class the prediction accuracy will be obviously greater than 50% and its misleading model which leads to failure in model selection and evaluation.

Here we show how to use two different methods to handle such imbalanced datasets:
1. Near Miss - technique which balances the dataset to the minority class - Undersampling
2. SMOTE - technique helps to oversampling of the minority class to creates a dataset having equal distirbuted classes

First method results in loss of information - so the accuracy will be lower and we run a risk of underfitting of the majority class.
Second method is efficient due to no loss of information only it takes time in training models and evaluting.

Here we use four types of classifiers to build predictive model:
1. SVC - Support vector classifier
2. Logistic Regression
3. k-NN 
4. Decision Tree

Tuning these models for model parameters using the gridsearch cross validation. 

Using ROC on test scores we choose the best model for the given dataset.

We found that Logistic Regression performs well for both undersmapling and SMOTE(Oversampling) technique with accuracy of 95%




