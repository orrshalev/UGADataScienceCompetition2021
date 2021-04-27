# University of Georgia Data Science Competition 2021: Project Overview
* Created machine learning models to predict the likelihood of default among credit card applicants.
* Worked with multidisciplnary team as team lead.
* Delivered Jupyter Notebook, written report, and oral presentation in contest.
* Won cash prize and presented findings in front of industry experts as runner-up.

## Code and Packages Used 
**Python Version:** 3.8.5

**Packages:** numpy, pandas, matplotlib, seaborn, sklearn, statsmodels, autoimpute 


## Competition Webpage
https://www.youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t

## EDA
Analysed disperities among defaulting and non-defaulting populations, checked if there is a sufficient observation count, and searched for collinearity and missing values. Below are a few highlights.
![alt text](https://github.com/orrshalev/UGADataScienceCompetition2021/tree/main/visualizations/confusion_matrices.png)
![alt text](https://github.com/orrshalev/UGADataScienceCompetition2021/tree/main/visualizations/uti_card_distribution.png)
![alt text](https://github.com/orrshalev/UGADataScienceCompetition2021/tree/main/visualizations/vif_table.PNG)

## Models Created
The competition entailed creating a Logistic Regression model and choosing from the following.
* XGBoost
* Random Forest
* Feedfoward Neural Networks

Random forest was chosen as the second model due to resiliancy to noise and relatively high interpretability.

## Model Building
**Logistic Regression:** some features were combined or dropped to maintain low collinearity. Missing values were removed as part of feature combination. Dummy variables were created for categorical variables.

**Random Forest:** missing values were imputed and features with low linearity to response variable were removed. Dummy variables were created for categorical variables.

GridSearchCV was used for hyperparameter optimization in both models.

## Model performance
Both models were fairly accurate.
*	**Logistic Regression** : 93.58%
*	**Random Forest**: MAE = 93.66%

## Model Choice
The random forest model was chosen due to stronger performence in classification of true positives and mitigation of type 1 error.
![alt text](https://github.com/orrshalev/UGADataScienceCompetition2021/tree/main/visualizations/roc_curves.png)
