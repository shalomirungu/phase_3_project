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
 **dummy model**
 It has an accuracy of approximately  86%, recall of 1, precision of 0.86, and f1 score of 0.92. However, the AUC of the model is 0.5, showing that it cannot differentiate between true and false classes.
 **Logistic regression model**
The model has an accuracy of  approximately 77%, recall of 0.69, precision of 0.34, and f1 score of 0.46. The training dataset has an AUC of 0.86, meaning that it has a high ability to differentiate between true and false classes. The testing dataset has an AUC of 0.79, showing that it performs well on unseen data.                                           
 **Decision Tree Model**
 It has an accuracy of approximately 85%, recall of 0.76, precision of 0.47, and f1 score of 0.58. It is a better-performing model than the logistic regression. However, the AUC of the training set is 1 and that of the testing dataset is 0.85, meaning that it has overfitting and requires tuning. The training set accuracy of the pruned decision tree becomes 85.44% and that of the testing set becomes 87.56%.  
 **Tuned decision tree model**
 It has an accuracy of 87.6%, recall of 0.76, precision of 0.54, and f1 score of 0.63. Training and testing set accuracy is 94.1% and 87.6% respectively, showing that there is still overfitting.
 **Random forest**
 It has training and testing accuracy of 91.48% and 92.20% respectively  
 **XGB Classifier**
 It has training and testing accuracy of 100% and 92.95% respectively but may be a sign of overfitting                                               
 **Tuned XGB Classifier**
 This is the best model, with training and testing set accuracy of 97.1% and 92.4% respectively  
                                                                              
