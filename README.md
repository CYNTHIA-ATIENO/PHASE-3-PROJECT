# PHASE-3-PROJECT

### PROJECT OVERVIEW
The primary objective of this project is to develop a predictive model that can classify whether a customer will stop doing business with SyriaTel in the near future. This will help SyriaTel proactively identify at-risk customers and implement retention strategies to reduce churn and minimize financial losses.

## DATA SOURCE
SyriaTel Customer Churn Data: The primary dataset used for this Analysis is the 'bigml_59c28831336c6604c800002a.csv' file, containing detailed information about each customer.
## TOOLS
-Python 

## 1. BUSINESS UNDERSTANDING
SyriaTel is a telecommunications company based in Syria. It is one of the largest and most established telecom providers in the country. SyriaTel offers a range of services, including:

Mobile Telephony: Providing cellular services such as voice calls, text messaging, and mobile internet.

Fixed-Line Services: Offering traditional landline phone services.

Internet Services: Including broadband and data services for both residential and business customers.

Value-Added Services: Such as mobile banking, entertainment services, and other digital solutions.

SyriaTel plays a crucial role in the telecommunications infrastructure of Syria, serving a broad customer base and contributing to the connectivity and communication needs of individuals and businesses in the region.

## 2. PROBLEM STATEMENT
SyriaTel aims to enhance its customer retention efforts by understanding and predicting customer churn. The goal is to create a machine learning model that predicts the likelihood of a customer discontinuing their services in the near future. By identifying high-risk customers early, SyriaTel can tailor personalized retention offers, improve customer satisfaction, and reduce revenue loss associated with churn.

This model will help the company proactively implement targeted retention strategies, thereby minimizing revenue loss and improving customer retention.
## 3.Objectives
1.Predict Churn: 

Develop a classifier to predict whether a customer will churn within the next 6 months based on their historical data and behavior..

2.Identify Risk Factors:

Determine the key factors and patterns associated with higher churn probability to inform targeted retention strategies.

3.Improve Retention Strategies: 

Provide actionable insights to SyriaTel for creating effective retention campaigns, such as personalized offers or improved customer service interventions.
## 4.Data Understanding:

This project uses the SyriaTel dataset whose size, descripritive statistics for all the features used in the analysis, and justification of the inclusion of features based on their properties and relevance for the project have been given in the Exploratory Data Analysis part.

The data contains all the relevant features that are needed to meet our objectives as described above.

However, to explain the relationship fully, additional features such as customer complains are needed.

## 5.Data cleaning and preparation

In this phase I perfomed the following tasks:
1. Loading and previewing the data
1. Handling Missing Values
2. Checking  Number of labels: cardinality
3. Encoding Categorical Variables
4. Finding the correlation between variables. I used Correlation Heatmap

 ## 6.Exploratory data analysis(EDA)
  EDA involves exploring the Syria Tel data to get answers to the following questions;
  1. Will the customer churn within the next 6 months?
  2. What factors contribute to customer churn?
  3. What strategies can the company use to imrpove customer retention?
     
 ## DATA ANALYSIS
1. I Defined features and target variable
 
2.Normalize/Scale Numeric Features

3. Split the Data into Training and Test Sets

4. Chose and Trained a Model

5. performed a clssification metric

6. model tuning- I used ROC-AUC

7. cross validation using Decision Tree

8. Hyperparameter Optimization using GridSearch CV

 ## 7. Result and Conclusion
1. The logistic regression model accuracy score is 0.852. So, the model does a very good job in predicting whether or not the cutomer will churn.

2. Small number of observations predict that customer will churn. Majority of observations predict that customer will not churn.

3. The model shows no signs of overfitting.

4. Overall Performance of the Decision tree model:

- The decision tree model shows high performance with a mean accuracy of 91%, which is quite good. This implies that the model is effectively capturing patterns in the data and making accurate predictions.
- Consistency:
The low standard deviation (0.02) suggests that the model’s performance is consistent across different folds of the cross-validation. This indicates that the model is not overly sensitive to the specific data it was trained on, which is a positive sign of robustness.

- Model Suitability:
Given the high mean accuracy and low variability, the decision tree model appears to be well-suited for this dataset. It is performing reliably and accurately.

5. Our original model test accuracy is 0.852 while GridSearch CV accuracy is 0.94. We can see that GridSearch CV improve the performance for this particular model.

## 8.LIMITATION

The regression model shows a lower rate of predicting true positives(53%) of customer churn. This might ,misinform the company if other superior modelas are not used.

#9.RECOMMENDATIONS
1. Leverage the Best-Performing Model
Adopt the Decision Tree model for primary churn predictions due to its higher accuracy and consistency.

Keep the Logistic Regression model as a secondary model to validate results or for scenarios where interpretability is crucial, given its simpler nature compared to Decision Trees.

2. Address Class Imbalance: There is a small number of observations predicting churn, indicating class imbalance.
I would recommend the use of resampling techniques or class weight adjustments

3.Validate Model Performance

Monitor and validate models regularly to ensure continued performance and adaptation.

4. Improved Performance with GridSearch CV: GridSearch CV improved the Logistic Regression model’s accuracy to 94%.
Recommendation;

Leverage GridSearch CV to optimize both models and refine feature selection.

5. Business Implications and Actions Implement actionable strategies based on model predictions to reduce churn effectively.
Churn Prediction Utilization: Use the high-performing models to proactively address customer churn. Implement strategies such as targeted retention campaigns, personalized offers, or enhanced customer service for those predicted to churn.

Resource Allocation: Allocate resources effectively based on model predictions to maximize the impact on customer retention.

6. Re-evaluate Models Periodically:
Regularly update models with new data and reassess their performance to ensure they remain effective as customer behaviors and market conditions change.



   

