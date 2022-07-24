# CIND820-Capstone
[CIND 820 Readme.docx](https://github.com/TejpreetBhatti/CIND820-Capstone/files/9003497/CIND.820.Readme.docx)


A Data-Driven Approach to find the Most Profitable and Engaged Customers for Insurance firms



Author: Tejpreet Bhatti

CIND820: Big Data Analytics Project

Dr. Sedef Akinli Kocak




# Repository Contents

This repository contains the code required to evaluate the impact of Customer Lifetime Value measures on the insurance industry within the United States utilizing a Decision Tree Model, a KNN Model, Random Forest, Multinomial Logistic Regression and a Naïve Bayes Model.




# Table of Contents

-Abstract

-Problem statement

-Data 

-Techniques and Tools

-Evaluation Metrics

-Repository Content

-Dataset

-Methodology

-Initial Results

-Results 

-Conclusion 





# Abstract

The core business of insurance companies is to protect people and businesses from extreme losses. Furthermore, insurance is an intangible good, that requires advance payment before it's used by the way of monthly payments. Over the past 20 years, insurance companies and companies from most all sectors have looked for ways to improve their customer portfolio by locating, attracting, and retaining the most profitable. For this to happen, companies needed to classify their customer into segments for current and future value. To measure high valued clients, most companies have adopted Customer lifetime value (CLV). The definition of CLV is the amount of money a customer will spend with a business in his/her lifetime.
The insurance industry is an extremely complex business because customer lifetime value and retention are always of the highest priority. The longer a customer stays with one company the higher the profits the company can reap. To analyze these phenomena, the IBM Watson dataset was collected to predict; what traits and behaviour do the most profitable customers exhibit. For an insurance company, the goal is to find and keep high-value customers that will provide the company profits for as long as possible.
This study aims to discover customers that provide the highest Customer Lifetime Value and factors that lead to a high-value customer. Specifically, it will help discover behaviour and characteristics of “what variables lead to a customer becoming high value to a company? what constitutes a high-value customer? what customer segments are the most profitable?” based on twenty-four demographic and industry-related variables. The “Customer Lifetime Value” column a raw dollar amounts, which means it is a regression problem. But for further analysis, those dollar amounts will be binned into low, medium, and high, which means this data could also be analyzed from a classification problem perspective.


# Problem Statement

The initial research question for this study is as follows:
What variables lead to a customer becoming high value to a company?
Additionally, this study will be exploring the use of machine learning for prediction within the domain of CLV in the insurance. Thus, this study has an addition research question as follows:
Through utilization of machine learning techniques, what constitutes a high-value customer? What customer segments are the most profitable?


# Data

The dataset used to solve the problem stated above comes from Kaggle; the name of the data set is IBM Watson Marketing Customer Value Data. The dataset has both categorical and integer/numeric attributes. The dataset has 9134 instances or rows. The dataset also does not have any missing values. This dataset also falls into the supervised learning category as it is predicting continuous and classified values. The dataset is biased because 85% of the customers are not engaged.


# Techniques and Tools

Python will be used across the lifecycle of this study. Three approaches will be adopted:
Decision Trees – will be used for model building and prediction. Chosen for its visualization ability,  comprehensive predictions and works great with multiclass problems.
KNN- will be used for model building and prediction. Chosen due to it can learn non-linear decision boundaries and it has a single hyperparameter the value of K.
Naïve Bayes – will be used for model building and prediction. Chosen due it works continuous and discrete data, very scalable number of predictors and data points and works great with multiclass problems
Randon Forest - will be used for model building and prediction. Chosen for its similarity to decision trees. Hence can compare the results with decision trees
Multinomial Logistic Regression - will be used for model building and prediction. Chosen for its ability to perform multiclass logistic regression 


# Evaluation

Model evaluation metrics will be:

Accuracy, Precision, Specificity, Confusion Matrix , F1 score and runtime will be calculated
Requirements
Python and R
Required packages are as follows:
Python: Pandas, Numpy, OS, Matplotlib.pyplot, Seaborn, Stasmodel.api, Scipy.stats
R: (rapportools), (tidyverse), (ggplot2), (RColorBrewer), (gridExtra), (corrplot), (corrgram), (arules), (arulesViz), (dplyr), (caret), (dplyr), (ggraph), (igraph), (factoextra), (purrr), (rpart) and (rattle)


# Repository Content

-Both capastone code.rmd and capstonepythoncode.ipynb is code for exploratory data analytics and descriptive statictics 

-CIND 820 Initial Code.rmd is code for data prep, data modeling and intial results 

# Datasets

IBM Watson Marketing Customer Value Data: https://www.kaggle.com/datasets/pankajjsh06/ibm-watson-marketing-customer-value-data 

The following variables are found in the dataset above:

## Policy Profile Variables
•	Customer: Customer ID number
•	Customer Lifetime Value: Customer's total worth to business over life of the relationship
•	Response: Yes or No response to a renewal offer
•	Coverage: Type of policy (Basic, Extended, Premium)
•	Monthly Premium Auto: Amount of customers' monthly insurance payments
•	Months Since Last Claim: Number of months between customers' last reported insurance claim
•	Months Since Policy Inception: Number of months since customer began an insurance policy
•	Number of Open Complaints: Number of unresolved customer complaints
•	Number of Policies: Number of policies customer currently owns
•	Policy Type: (Corporate Auto, Personal Auto, Special Auto)
•	Policy: 3 levels (L1, L2, L3) per Policy Type (Corporate, Personal, Special)
•	Renew Offer Type: 4 types of renewal offers (Offer 1, Offer 2, Offer 3, Offer 4)
•	Sales Channel: Channels to purchase a policy (Agent, Branch, Call Center, Web)
•	Total Claim Amount: Cummulative amount of claims since policy inception


## Customer Profile Variables
•	State: State of residence or business
•	Education: Level of education (High School or less, College, BA, MA , PHD)
•	Effective To Date: Date the policy expires
•	Employment Status: (Employed, Unemployed, Retired, Disabled, Medical Leave)
•	Gender: Male or Female
•	Income: Customers' annual income
•	Location Code: (Rural, Suburban, Urban)
•	Marital Status: (Single, Married, Divorced)
•	Vehicle Class: Type of vehicle (4-Door, Luxury, Luxury SUV, Sports Car, SUV, 2-Door)
•	Vehicle Size: (Large, Midsize, Small)





# Methodology

The study methodology was as follows:

Step	Description

PROBLEM AND OBJECTIVE DEFINITION: Identify business context, define problem and related objectives.

DATA COLLECTION: Dataset was gathered, merged and organized in similar time periods by IBM Watson. 
DATA PREP & PREPROCESSING 	Data cleaning (duplication elimination, missing value detection, error detection, outlier detection), transformation, normalization, discretation and dimensionality reduction/feature selection 

DATA EXPLORATION: Descriptive statistics, univariate analysis, bivariate analysis data visualization (generate graphs and charts). Purpose to find trends, patterns and correlations

DATA MODELING: Split model into training and testing sets, conduct predictive analysis. Perform Decision tree, KNN, Random Forest, Multinomial Logistic Regression and Naïve Bayes algorithms. Perform 10-fold cross-validation.

MODEL EVALUATION: Present results for all models including all evaluation metrics. Accuracy, Precision, Specificity, Confusion Matrix, F1 score and runtime will be calculated.

INTERPRET & COMMUNICATE:	Interpret results against evaluation metrics and present findings (report, presentation etc.).



# Initial Results

The following 3 models were built and evaluated: • Decision Trees • KNN • Naïve Bayes

Summary performance measures for each model is as follows:


Model	                 | Decision Tree	 |     KNN	     |     Naïve Bayes |
-------------------------|-----------------------|-------------------|---------------- |
Accuracy	         |         0.94	         |     0.62	     |       1         |                                                  
Recall(Sensitivity) -Low |         0.97          |     0.67          |       1         |
Recall(Sensitivity) -Avg |         0.90          |     0.59          |       1         |
Recall(Sensitivity) -High|         0.94	         |     0.60          |       1         |                         
Precision - Low	         |         0.98          |     0.63          |       1         |
Precision - Avg          |         0.89          |     0.65          |       1         |
Precision - High         |         0.93	         |     0.58          |       1         |	                
F1-score - Low 	         |         0.98          |     0.65          |       1         |
F1-score - Avg 	         |         0.89          |     0.62          |       1         |
F1-score - High 	 |         0.93          |     0.59          |       1         |                       
Specificity - Low 	 |         0.99          |     0.76          |       1         |
Specificity - Avg        |         0.95          |     0.87          |       1         |
Specificity - High       |         0.97	         |     0.80          |       1         |	                
Training time	         |         8.46s         |    0.21s	     |      1.24min    |
Prediction time	         |         0.15s	 |    2.2s	     |      12.31s     |


# Final Results

The following 5 models were built and evaluated: • Decision Trees • KNN • Naïve Bayes • Random Forest • Multinomial Logistic Regression

Summary performance measures for each model is as follows:

Model	                 | Decision Tree	 |     KNN	     |     Naïve Bayes |        Random Forest | Multinomial Logistic Regression |
-------------------------|-----------------------|-------------------|---------------- |--------------|-------------------------------|
Accuracy	         |         0.92	         |     0.52	     |       1         |      0.92      |    0.68     |                                            
Recall(Sensitivity) -Low |         0.97          |     0.53          |       1         |    0.96    |   0.83   |
Recall(Sensitivity) -Avg |         0.90          |     0.59          |       1         |    0.95    |   0.69   |
Recall(Sensitivity) -High|         0.84	         |     0.41          |       1         |    0.84    |   0.43   |             
Precision - Low	         |         0.98          |     0.56          |       1         |    0.98    |   0.64   |
Precision - Avg          |         0.88          |     0.52          |       1         |    0.97    |   0.77   |
Precision - High         |         0.98	         |     0.48          |       1         |	  0.93    |   0.60   |        
F1-score - Low 	         |         0.97          |     0.54          |       1         |    0.97    |   0.72   |
F1-score - Avg 	         |         0.89          |     0.55          |       1         |    0.90    |   0.73   |
F1-score - High 	 |         0.86          |     0.43          |       1         |          0.88    |   0.50   |        
Specificity - Low 	 |         0.99          |     0.74          |       1         |        0.99    |   0.71   |
Specificity - Avg        |         0.92          |     0.66          |       1         |    0.92    |   0.88   |
Specificity - High       |         0.96	         |     0.86          |       1         |	  0.98    |   0.91   |           
Training time	         |         17.27s         |    0.24s	     |      1.24min    |  3.63s           |   2.86s  |
Prediction time	         |         0.21s	 |    1.5s	     |      12.31s     |    0.26s             |   0.09s  |

# Study Conclusions

This study explored the relationship between demographic/ policy variables and customer lifetime value. The research questions focused on determining which variables significantly affect the customer lifetime value as well as which variables are able to predict the customer lifetime value.  Five models were built using Decision Trees, KNN, Naïve Bayes, Random Forest and Multinomial Logistic Regression. The models were able to identify relationships between demographic/ policy variables and customer lifetime value helpfully a significant relationship was established. The following variables (number of policies, policy type, total monthly premium, marital status, age, employment status, age, vehicle and class/size) had the biggest impact of customer lifetime value, demonstrating that key demographic/ policy variables fully describe CLV. The decision tree and random forest outperformed KNN, naïve bayes and multinomial logistic regression model by a significant margin and were able to provide better predictive performance.
This study contributes to the body of knowledge regarding the impact of demographic/ policy variables on the CLV in the insurance industry. It identified that, (number of policies, policy type, total monthly premium, marital status, age, employment status, age, vehicle and class/size) will impact to CLV, there are many factors outside the realm of dataset could also impact CLV. Additionally, a solid relationship between demographic/ policy variable and CLV was concluded, however additional research may be required. Demographic variables were found to have a greater impact on predictive performance than policy variables
Further studies within this area can focus on exploring the relationship between customer residence (state/zip code)focused on CLV in the insurance industry. Studies can additionally explore the relationship between aggregate regression models instead of classification models and their predictive performance in relation to the CLV in the insurance industry.
