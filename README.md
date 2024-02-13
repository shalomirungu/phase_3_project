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
 This is the best model, with training and testing set accuracy of 97.1% and 92.4% respectively. The following are a confusion matrix and ROC curve for the XGB classifier:
 
![2024-02-13 (1)](https://github.com/shalomirungu/phase_3_project/assets/149403427/480d7347-ba5d-49cd-849b-93d1bee2df2f)
 
 ### Significant predictors for customer churn
 Total day charge, Voice Mail Plan, Area Code 415 and Area Code 510, Customer Service Calls, Number of Voicemail Messages, International Plan, Total Day Minutes, Total International Calls, Total Evening Minutes, Total International Minutes. The following is a graph representing the order of significance:
 ![2024-02-13](https://github.com/shalomirungu/phase_3_project/assets/149403427/5524fb90-eb23-4ba9-ac16-fb9975f22a21)
 
 ## Conclusion and Recommendations 
 The XGB model is the best as it had the best performance on both the training and testing sets. From this model, we recommend that:
 1. Targeted pricing strategies, discounts, or loyalty programs are implemented to manage and reduce total day charges for customers at risk of churn.
 2. Personalized offerings or promotions for international services are considered to align with the customers' needs.
 3. Voicemail services are evaluated and enhanced, considering additional features or personalized messaging to increase customer engagement.
 4. A detailed analysis of customer behaviors in different areas is done to ensure implementation of region-specific strategies or promotions to address localized concerns.
 5. Educational campaigns are launched to inform customers about international plan benefits and usage tips.
 6. The predictive model is constantly updated  based on new data to ensure its continued accuracy.
 7. A robust feedback mechanism is established to gather insights directly from customers.
                                                                              
