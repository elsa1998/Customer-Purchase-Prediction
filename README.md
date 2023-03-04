# Customer-Purchase-Prediction
Use deep learning and ensembling models to predict customer spending (on all data & purchasing data)

## About Data
This dataset is about whether or not different consumers purchase in response to a test mailing of a certain catalog and, how much money each consumer spent. This dataset has two possible outcome variables: Purchase (0/1 value: whether or not the purchase was made) and Spending (numeric value: amount spent).

## Goal
Build numeric prediction models that predict Spending based on the other available customer information.

## Exploratory Data Analysis
Distinct the categorical and numerical columns, Normalization

## Modeling (a): all data & Modeling (b): Purchase = 1
- Split training and testing set
- Score = MSE
- Cross-validation for inner and outer loops
- Hyper parameter tuning on linear regression, K-NN, Regression tree, SVM regression
- Ensembling models: stacking, and tune hyperparameter in regression tree
- Modeling: Neural Network
- Compare MSE score between 5 models

## Result
- For the whole data, KNN model has the lowest MSE (-18087) 

{'linear regression': -18335, 'KNN': -18087, 'Regression tree': -20913, 'SVR': -20894, 'Stack': -20376}

- For the purchasing data, linear regression model has the lowest MSE (-27487)

{'linear regression': -27487, 'KNN': -53244, 'Regression tree': -32879, 'SVR': -51678, 'Stack': -29873}
