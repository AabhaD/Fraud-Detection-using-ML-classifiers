# Fraud Detection using ML classifiers

## Executive Summary
Banks are required to report suspected vulnerable (elder and dependent adult) financial exploitation. As digital payments continue to expand across all demographics, research shows that older adults are showing the biggest uptick in adoption during the 2020/21 period due to the pandemic. Banks are required to report elder financial abuse but, unless a customer reports fraud and files a claim, financial abuse can go undetected and repeated fraud via digital payments can continue without the banks’ knowledge. Without detection models, a large amount of fraud is left unreported by consumers and elder and vulnerable adult populations will be at greater risk of being targeted and losing savings to fraudulent payments. As the older adult segment continues to adopt digital technology, including digital payments, banks need better ways to predict and analyze transaction data to detect high risk payment patterns or transaction attributes that signal high risk for fraud, especially for older and vulnerable adult customers, which could be targeted by scammers.

## Data and Packages/skills used -
- Data : [This data was provided by Wells Fargo Campus Analytics Challenge conducted by mindsumo](https://www.mindsumo.com/contests/campus-analytics-challenge-2021)
- Programming Language : Python 
- Packages : pandas, numpy, matplotlib, seaborn, sklearn

## Data cleaning
Missing values were imputed and data types were formatted to make the data usable for machine learning models.

## EDA
Count for Fraud and Non-Fraud cases
![](

Types of devices used to initiate fraudulent transaction
![](

## Model Building
- ML models used : KNN Classifier, Logistic Regression Classifier, SVM, Decision Tree, Random Forest


## Model Performance
ROC Curve for Decision Tree Classifier
![](

## Conclusion :
We get **maximun roc_auc_score: 0.9694 by using Decision Tree Classifier** with 'max_depth': 5, 'min_samples_leaf': 90, 'min_samples_split': 250. Also from Auc_roc curves we observe that the decision tree curve is close to top left as comparared to other models. This also proves that area under the curve, AUC is higher for the Decision Tree Classifier. Hence this is the best model to predict suspected elder fraud in the digital payments space.

