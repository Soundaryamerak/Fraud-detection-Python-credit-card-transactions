# Fraud Detection using Python
Determining the best ML model for fraud detection on credit card transactions using Python.

## Data
The dataset contains transactions made by credit cards in September 2013 by European cardholders. It includes 284,807 transactions and 28 features after performing PCA. [Dataset from here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## ML Models Used:

- Logistic Regression
- Random Forest Classifier

**[Python File](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/blob/main/Fraud%20Detection.ipynb)**

## Understanding the Data

1. The dataset includes 31 columns: 28 features (V1 to V28), Time elapsed (sec), Amount, and Class.
2. The Class (target variable) is 0 or 1, indicating non-fraudulent and fraudulent transactions. There are 492 fraudulent and 284,315 non-fraudulent activities.

    ![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/72ee2b5c-dd07-4515-8ae5-3adb6757b324)

3. The majority of fraudulent transactions are for amounts between 0-500. Specifically, 113 (23%) of them are for the amount 1.
    ![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/28c3cd0e-9c0f-4bf1-a5e7-df073e07efef)
    ![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/c7c56b07-17c7-46cc-9004-00a08473b4a3)

4. There are no missing values, as indicated by the heatmap.
    ![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/1fae9bab-fd91-4b7b-bce5-8056f55edfa3)

5. No highly correlated variables are observed from the correlation matrix.
    ![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/3f84f3d4-5d45-4dce-8edf-3c3af1403f20)

## Performance Comparison

![image](https://github.com/Soundaryamerak/Fraud-detection-Python-credit-card-transactions/assets/170541567/6cb959e9-296b-4e21-a41e-2d4ffd21d3fc)

## Analysis

- **Accuracy:** All models have very high accuracy, with the Random Forest classifiers slightly outperforming Logistic Regression.
- **Precision and Recall (Class 1):** The Random Forest classifiers show significantly higher precision and recall for the minority class (Class 1), indicating better performance in detecting fraud.
- **F1-Score (Class 1):** The F1-scores for the Random Forest classifiers are also higher, suggesting a better balance between precision and recall compared to Logistic Regression.

## Conclusion
The Random Forest Classifier models, especially the tuned version, are better in terms of detecting the minority class (fraud cases) as they have higher precision, recall, and F1-scores for Class 1 compared to the Logistic Regression model.

## Steps Taken in Python

1. Import all necessary libraries (matplotlib, seaborn, pandas, numpy, Scikit-learn (Sklearn - model selection, linear model, preprocessing, metrics), imblearn, collections).
2. Understand the data available with visualization.
3. Split the data into train & test samples.
4. Train & evaluate the Logistic Regression model.
5. Downsample data to optimize results.
6. Split data into train & test samples again.
7. Train the Random Forest Classifier model.
8. Test & evaluate the Random Forest model.
9. Hyperparameter tuning of the Random Forest model.
10. Evaluate the Random Forest model again.
11. Compare results.
