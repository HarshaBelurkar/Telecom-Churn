# Telecom-Churn

Problem Statement

In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another.To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. In this project, we will analyse customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn and identify the main indicators of churn.Churn prediction is usually more critical for prepaid customers.We need to use the usage-based definition to define churn.

High Value Churn

In the Indian and the southeast Asian market, approximately 80% of revenue comes from the top 20% customers (called high-value customers). Thus, if we can reduce churn of the high-value customers, we will be able to reduce significant revenue leakage.
In this project, we will define high-value customers based on a certain metric and predict churn only on high-value customers.

Model Approach

Build models to predict churn. The predictive model that we are going to build will serve two purposes:
It will be used to predict whether a high-value customer will churn or not, in near future (i.e. churn phase). By knowing this, the company can take action steps such as providing special plans, discounts on recharge etc.
It will be used to identify important variables that are strong predictors of churn. These variables may also indicate why customers choose to switch to other networks.

Business Objective

The business objective is to predict the churn in the last (i.e. the ninth) month using the data (features) from the first three months

Detailed Steps Followed while building the model

1. Preprocess data (convert columns to appropriate formats, handle missing values, etc.)
2. Conduct appropriate exploratory analysis to extract useful insights (whether directly useful for business or for eventual modelling/feature engineering).
3. Derive new features.
4. Reduce the number of variables using PCA.
5. Train a variety of models, tune model hyperparameters, etc. (handle class imbalance using appropriate techniques).
6. Evaluate the models using appropriate evaluation metrics. Note that is is more important to identify churners than the non-churners accurately - choose an appropriate evaluation metric which reflects this business goal.
7. Finally, choose a model based on some evaluation metric.
8. Finally, recommend strategies to manage customer churn based on our observations

The first model will only be able to achieve one of the two goals - to predict customers who will churn. You can’t use the above model to identify the important features for churn. That’s because PCA usually creates components which are not easy to interpret.
Therefore,we need to build another model with the main objective of identifying important predictor attributes which help the business understand indicators of churn. A good choice to identify important variables is a logistic regression model or a model from the tree family. In case of logistic regression, make sure to handle multi-collinearity.
