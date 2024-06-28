# Fraud-detection on Python
Determining the best ML model for Fraud detection on credit card transactions using Python

# Data
The dataset contains transactions made by credit cards in September 2013 by European cardholders. 284,807 transactions and 28 features after perfoming PCA [From here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

# ML models used:
Logistic Regression & Random Forest classifier

# Steps taken in Python
1. Import all necessary libraries (matplotlib, seaborn, pandas, numpy, Scikit-learn (Sklearn - model selection, linear model, preprocessing, metrics), imblearn, collections.
2. Understand the data available with visualisation
3. Split the data in train & test sample.
4. Train & evaluate Logistic regression model
6. Downsampling data to optimize results
7. Split data into train & test sample
8. Train Random Forest Classifier model
9. Test & Evaluate RF model
10. Hyperparameter tuning of RF model
11. Evaluate RF model again
12. Comparing results

# Understanding the data
**Number of variables**
1. There are a total of 31 columns, 28 of them features (v1 to v28), Time elapsed (sec), Amount and Class.
2. Class (target variable) is 0 or 1, for non-fraudulent and fraudulent transaction. 492 fraudulent and 284315 non-fraudulent activities.

    ![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/72ee2b5c-dd07-4515-8ae5-3adb6757b324)


3. Majority of fraudulent transactioins are of amounts between 0-500. Specifically, 113 (23%) of them are of the amount 1.
![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/28c3cd0e-9c0f-4bf1-a5e7-df073e07efef)
![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/c7c56b07-17c7-46cc-9004-00a08473b4a3)


5. There are no missing values as indicated by the heatmap

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/1fae9bab-fd91-4b7b-bce5-8056f55edfa3)

6. No highly correlated variables as observed from the correlation matrix.

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/3f84f3d4-5d45-4dce-8edf-3c3af1403f20)

# Evaluation of Logistic regression model
*Accuracy: 0.9992225276378884*

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/a709603b-6ab5-49c2-b240-aa8aaaef6534)

# Data after Downsampling

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/23157d51-2525-42ce-b361-8f76a8dc4e02)

# Evaluation of Random forest classifier model

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/635f8df3-a6f3-40ae-a90f-5b4c0685ef22)

# Evaluation of Random forest classifier model after hyperparamater tuning

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/9eb090f2-00b8-4cc3-b091-f62aa4c1fab6)

# Comparing results





