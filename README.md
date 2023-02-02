
# Title of Project



![1_Lci4cCUXgb6zZRyKmgWfVA](https://user-images.githubusercontent.com/114376944/216277722-504b5822-e7a2-4229-b929-846d3eb6a781.png)

### Credit Card Fraud Detection Project


# Introduction
This project is aimed at detecting fraudulent activities on credit cards. Credit card fraud is a major issue affecting millions of customers and financial institutions globally. The objective of this project is to build a model that can accurately identify fraudulent transactions based on transaction data.

## Problem Understanding
Credit card fraud is becoming increasingly. It becomes major concern for credit card holders and credit card issuers. Scammers uses others credit card for financial transaction and other persons have not knowledge about it.
Credit card holder can suffer from financial loss. Not only the credit card holders but the credit card issures also experience singificant loss like demaging their reputation and loosing customer trust.

To prevent these losses credit card fraud detection is required. By using machile larning algorithm and AI credit card companies can identify and prevent these fraud before occuring.
## Data 
The data set contains the transactio by credit card in sep 2013 by Europen card holders. This dataset present transaction that occured in two days where we have 492 faud out of 284802 transactions. The data is highly unbalanced
It contains only numerical variable which are the result of PCA transformation. Due the confidentiality original features are not provided. 
The data set contains total 31 columns out of them 28 (V1 to v28) are transformed by PCA, and 1 is target columns

The data set is downloaded from kaggle.


To downlad the data set you can refer to this link:-

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

![credit_card_fraud](https://user-images.githubusercontent.com/114376944/216277846-763a6b15-07c9-410e-a588-c711b39541a8.PNG)


## Prerequisites
The following packages and libraries are required to run this project:

- Python 3.x
- Pandas
- NumPy
- Sklearn
- Matplotlib
- Seaborn
- imbalanced-learn
## Task Done

- Problem Undertsatnding and Data Collection part are already Done 

### 1) EDA
- After reading the data set we have done Exploratory Data Analysis
- No null value is there in data set
- All the features are numerical in nature
- Done the statistical Analysis
- See the distribution of data set
- outliers are present in data set
- Data set is very unbalanced



 ### 2) Fetaure Engineering 
#### a) outliers
 - Remove the outliers using IQR method

#### b) Handle unbalance data
- To handle unbalance data we have used two techniques
-  1.--Undrsampling
-  2.--Over sampling

#### c) Feature Scaling 

 - All the features excepting Time and Amount are result of PCA Transformation.
 - SO we have scaled the Time and Amount also using Robust scaler 

### 3) Model Building 
- First of all we have already split the data into train and test data set
- Trained multiple models on training data set like logistic regresion, Decision Tree classifer, Random forest classifier, XGBClassfier

### 4) Model Evaluation
- To evaluate the models multiple metrices are used like accuracy_score, cross validation score, classification report, recall, precission, ROC-AUC curve
- Compared the performance of models on the basis of cv_score or r2 score
- After evaluation we got XGBClassifier is giving the best best result.
 - So we finalize this model as best performing model among other used models.

#### Done some prediction using XGBRegressor



## Conclusion

The credit card fraud detection project is a crucial step in combating financial fraud. This project demonstrates that machine learning algorithms can be used to accurately identify fraudulent transactions.
## Future work

- We can also do hyperparameter tuning by using Grid Search CV or Random Search CV to find out best parameters
- We can also apply deep learning algorithm.
- After testing we will deploy the model
