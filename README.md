# Credit Risk Analysis

## Overview of the Analysis

The purpose of this analysis is to build a machine learning model that can help predict credit risk. By leveraging historical lending activity data from a peer-to-peer lending services company, we aim to identify the creditworthiness of borrowers. This project entails preprocessing data, splitting it into training and testing sets, and then implementing a logistic regression model to classify the risk associated with the loan status.

## Split the Data into Training and Testing Sets

- **Accuracy Score**: The model with the original data has an accuracy score of `99%`, indicating the overall correctness of the model across both classes.
- **Precision Score**: 
  - For healthy loans (0): `1.00` (indicating no false positives for healthy loans)
  - For high-risk loans (1): `0.84` (indicating a low rate of false positives for high-risk loans)
- **Recall Score**: 
  - For healthy loans (0): `0.99` (indicating a high rate of true positives for healthy loans)
  - For high-risk loans (1): `0.99` (indicating a high rate of true positives for high-risk loans)

## Create a Logistic Regression Model with the Original Data

After training our logistic regression model with the original data:

- **Accuracy Score**: The model’s accuracy was `0.9935981855334257`, reflecting its effectiveness in predicting loan status.
- **Precision Score**: Precision for healthy loans was perfect at `1.00`, while for high-risk loans, it was `0.84`.
- **Recall Score**: Recall for healthy loans was `0.99`, showing a high ability to identify true positives, and for high-risk loans, it was also high at `0.99`.

## Summary

The logistic regression model provides a reliable method for predicting credit risk based on historical data. With high scores in precision and recall, particularly after resampling the data to address class imbalance, the model demonstrates robustness in distinguishing between healthy and high-risk loans. As such, it is a valuable tool for the peer-to-peer lending services company to assess the creditworthiness of borrowers.

However, the performance metrics indicate there may still be room for improvement, particularly in the precision and recall for high-risk loans. Further model tuning, feature engineering, or even exploring more complex algorithms could potentially enhance the predictive performance. Nonetheless, the current model serves as a strong baseline for credit risk assessment.
