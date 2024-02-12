# Home_Credit_Default_Risk_prediction
### The purposes of this project is:  
1. To tinker with Machine Learning models, with a more focus on seeing how different models perform in complex datasets. Take a look at the [***8C. Models comparison:***](https://github.com/DannyQN123/Loan_Default_Risk_Analysis/tree/main?tab=readme-ov-file#8c-models-comparison) section for more detail. 
2. Look inside these Machine Learning models to derive any interesting insights. Take a look at section [***8D. Some insights - Using feature importance by machine learning model:***](https://github.com/DannyQN123/Loan_Default_Risk_Analysis/tree/main?tab=readme-ov-file#8d-some-insights---using-feature-importance-by-machine-learning-model) for more detail. Machine Learning models can provide some interesting insights.   
3. Along the way, try to find some interesting business insights within these data. Take a look at [***section 4 to section 6***](https://github.com/DannyQN123/Loan_Default_Risk_Analysis/tree/main?tab=readme-ov-file#4-factor-1-age). These are some of the insights by using Correlations between Default Rate & various factors like Ages, Income over Annuity Ratio and such.

## Big Question: 
- What are the factors that influence Home Credit customers' repayment ability ?
- This is a Binary-Classification problem.
- See the **Steps** & **Presentation** flow below for further detail. 


## Steps: 
1. Identify top 4 factors that affect a customer's repayment ability based on correlation (2 are given, 2 are engineered feature)
2. From 1 of the factor (Age), derive some actionable business insights using plotting (density plot, bar charts....)
3. Derive some more insights from 3 remaining factors that can help business make better decision
4. Evaluate the 3 Machine Learning models to derive some insights: What factors are most predictive of customer's ability to repay debt ?

## ROC AUC Score (as the measurement of predictive power) of different models
- Baseline are baseline models without adding engineered features. (So additional engineered features do help improve the predictive power of the model)  

![Screenshot (32)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/e03257de-0fd7-460f-91dc-8750c14adf45)

## Presentation flow
This is my presentation flow of the project 

### 1. Project Big Questions and Target Audience, Business overview

![Screenshot (55)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/35b52b45-b33a-448d-a43c-a3258d27d020)
![Screenshot (56)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/17b10d6b-ce12-40d2-9fb6-3925fea66fd5)

### 2. Product overview & Dataset Overview

![Screenshot (57)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/4667cc61-cac0-44cb-ba48-0c6cb957d7f3)

### 3. Dataset Schema, Presentation flow  

- Dataset for this task is provided plenty, so we will focus only on the 2 datasets in Red Redtangle below.
- Other dataset can be looked at in the future.

![Screenshot (58)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/37c1fbf6-f55f-4508-b4cd-76ffaa76c055)
![Screenshot (59)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/6366a330-73cd-446d-a120-bbf5a2c71b7b)

### 4. Factor 1: Age

![Screenshot (60)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/91db019d-d0e4-48b5-83f3-677f46fec03c)
![Screenshot (61)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/933bfbde-0f9b-40e6-84ff-78ae71e87703)
![Screenshot (62)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/ab1db301-d399-4357-94f8-5dd01cdb211e)

### 5. Factor 2: External Credit Score

![Screenshot (63)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/2a7dc93e-1fe5-4534-9af8-1c2e4c06477b)
![Screenshot (64)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/ad5a9a23-27b8-4840-a656-815a118ddad7)

### 6.  Factor 3 & 4: Credit Term & Income Annuity Ratio

![Screenshot (65)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/eef909aa-2393-4fbd-ae7a-76203cad6bf6)
![Screenshot (67)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/571ed51f-5834-4232-b9da-41873c070d93)
![Screenshot (68)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/a2255742-add4-401f-99e4-4d06f9f027e2)
![Screenshot (69)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/48904444-47b7-434b-afea-5b4b369764af)

### 7. Use machine learning for insights analysis: What features of customer is used most by Machine Learning models to determine the probability of them defaulting on loans ?  
- (meaning: Possibly a customer's age is influential on the probability of default, according to a machine learning model ? As in, ***older customer tends to less likely to default on loans ?***) 

![Screenshot (70)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/909470dc-d605-47d9-b5a2-9bbb31ba89dd)

### 8A. Prediction Probability:  
- Means the probability of default on loan predicted by Machine learning models (so if the model predict 0.268, this means that there is a 26.8% that this person will default on loans)  
### 8B. Input 123 features into machine learning models:   
- Putting too many features into ML model like this means sacrificing interpretability, but the aim is to alternatively demonstrate that when dataset becomes complex, ***tree-based model*** is better at capturing complex patterns, judging by ROC metrics.  

![Screenshot (71) (2)](https://github.com/DannyQN123/Loan_Default_Risk_Analysis/assets/107457149/6c49394c-fb3f-43e2-bc7d-3b743a8316b7)

### 8C. Models comparison:  
- As said above, tree-based models (Random Forest and LGBM) performs much better than Logistics Regression, judging by ROC AUC score.

![Screenshot (72)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/50f4e1b3-9ac6-429b-baf4-eca7ea8c42f2)
### 8D. Some insights - Using feature importance by machine learning model:  

- Looking at the ***feature importance*** by LGBM model (measured by number of splits - meaning how many time the model use this feature (e.g age of a customer, credit score of a customer)) to make decisions between - whether the customer going default or not.  

- We can see that the model use previous ***credit-scores*** (from other loan institutions - the name being ***ext_source_1 ,2 ,3***), among other top features, of customers many times **to make decision** whether they will default or not.   

- This make sense ***under business perspective***, being that customer's ***previous credit-scores*** are good indicators of whether they will be able to repay the current loans they have with Home-Credit     
- Also, according to the model, the ratios calculated by us ***(Credit Term & Income/Annuity Times)*** are also good indicator of whether the customer will default or not.  
- Further insights can be observe from these slides below, features like age, days_employed (how long have they been employed),.....of customers effect on their repayment ability.  

![Screenshot (73)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/c57dfab0-d4bd-4775-b765-bf686be199e3)
![Screenshot (74)](https://github.com/DannyQN123/Home_Credit_Default_Risk_prediction/assets/107457149/c24be424-879b-4f65-b7e6-9f8ab9942044)


