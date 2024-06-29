# Fraud-detection on Python
Determining the best ML model for Fraud detection on credit card transactions using Python

## Data
The dataset contains transactions made by credit cards in September 2013 by European cardholders. 284,807 transactions and 28 features after perfoming PCA [From here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## ML models used: 

**[Python File](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/blob/main/Fraud%20Detection.ipynb)**

Logistic Regression

Random Forest classifier

## Understanding the data

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



## Performance Comparison

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/6cb959e9-296b-4e21-a41e-2d4ffd21d3fc)

## Analysis

**Accuracy:** All models have very high accuracy, with the random forest classifiers slightly outperforming logistic regression.

**Precision and Recall (Class 1):** The random forest classifiers show significantly higher precision and recall for the minority class (Class 1), indicating better performance in detecting fraud.

**F1-Score (Class 1):** The F1-scores for the random forest classifiers are also higher, suggesting a better balance between precision and recall compared to logistic regression.

## Conclusion
The Random Forest Classifier models, especially the tuned version, are better in terms of detecting the minority class (fraud cases) as they have higher precision, recall, and F1-scores for Class 1 compared to the Logistic Regression model.

## Steps taken in Python
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
