# Credit-Card-fraud-prediction
Explored and visualized several datasets of credit card transactions using pandas and matplotlib. Improved the existing isolation forest algorithm using c.45 decision trees, which led to an increase in the recall metric of anomalies from 86% to 92%.

This repository contains Credit card fraud detection algorithm using machine learning techniques in python.

Credit Card Fraud Detection : With a lot of people, banks and online retailer being a victim of credit card fraud, a model detecting whether the transaction is fraud or not can help in saving a huge amount of money.

Dataset : The dataset has been obtained from kaggle. This dataset contains 284807 rows and 30 numeric columns and one class that specifies whether the transaction is fraudulent or not. The values of columns V1-V28 in the dataset may be result of a PCA(Principal Component Analysis) Dimensionality reduction to protect user identities and sensitive information. There are no missing values in the dataset.

Algorithm : The algorithm used in this dataset is Random Forest algorithm. For model improvement normalization and SMOTE techniques (to handle imbalanced data) were used.

Visualisation : The library used for visualizing the data, confusion matrix etc. is seaborn.

This code is prepared using Jupyter Notebook.

You can find the dataset in the link provided below: https://www.kaggle.com/mlg-ulb/creditcardfraud





Using simple logistic regression to predict credit card fraud transactions. Data set obtained from: https://www.kaggle.com/dalpozz/creditcardfraud

Data Set: creditcard.csv classes (column 31) are strings and csvread assumes numerical data, so I preprocessed a little by changing all class identifiers (e.g. "0", "1") to numerical 0 or 1. Easy to do in vim, run:
```
:%s/,"0"/,0/gi
:%s/,"1"/,1/gi
```

## Execute: run ccDriver.m

## UPDATE: So far 86% Precision, 80% Recall, and 99.9% overall accuracy

### TODO List:
```diff
+ Created under-sample of data for data-skew classification
+ Trained logistic regression classifier with under-sample data
+ Added precision/recall analysis
+ Executed multiple iterations per value of lambda (10000 for under_sample, and 3000 for entire data set)
- Graph learning curves to detect bias/variance issue (WIP)
- Use SMOTE and RF to push precision/recall to 98%+ (WIP)
````
