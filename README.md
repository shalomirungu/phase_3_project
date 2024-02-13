# **PREDICTION OF CUSTOMER CHURN**
# **Authors;** Immaculate Mwendwa, Shalom Irungu, Stephen Kariuki, Stella Ndegwa, Muhsin Ahmed and Joan Wambua.
## Project Overview
### Business Problem
SyriaTel is a popular telecommunications company faced with the problem of customer churn, whereby, customers no longer see fit to work with the company. This is caused by various factors such as stiff competition from other telecommunications companies and the challenge of constantly enhancing its services to boost customer experiences in the rapidly changing market. We focus on helping SyriaTel understand the factors that cause customer churn and provide a predictive model that helps identify customers who are most likely to leave, enabling the company to proactively deal with the situation at hand.
#### Objectives
* To **Identify the key features that predict Churn.**
* To **Investigate how to improve Customer Satisfaction.**
* To **Enable Strategic Decision-Making.**
* To **Predict customer churn.**
### Data
The data used is from SyriaTel customer records. It has 3333 customers and 21 features.
## Data Preparation
We checked for null values, normalized the target, modified the column names, and separated numerical and categorical variables.
## Exploratory Data Analysis
We visualized the target(churn) using a pie chart, and the categorical and numerical predictor variables using bar charts and subplots to understand their distributions. We also performed one-hot encoding and label-encoding of the categorical variables.
## Data Splitting and Class imbalance
We first split the data into training and testing datasets, then used the SMOTE technique to deal with class imbalance in the target variable.
## Modelling
We performed the following machine learning models: **a baseline using a dummy model**
                                                    **Logistic regression model**
                                                    **Decision Tree Model**
                                                    **Tuned decision tree model**
                                                    **Random forest**
                                                    **XGB Classifier**
                                                    **Tuned XGB Classifier**
We evaluated the precision, accuracy, recall, and f1 scores for these models.
## Modelling Results
