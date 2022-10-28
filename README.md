# Fraud-Detection - 
The challenge is to develop a machine learning model to predict suspected elder fraud in the digital payments space.

# Executive Summary
Banks are required to report suspected vulnerable (elder and dependent adult) financial exploitation. Today, much of this activity is limited to human interaction (bankers working with customers on the phone or in person), through which bankers may pick up queues, or red flags or customers self-reporting scams or financial abuse to their financial institution. Digital payments have a degree of reported fraud and claims, with the assumption that much more unreported losses occur, especially perpetrated against older adults (60 years of age or older). As digital payments continue to expand across all demographics, research shows that older adults are showing the biggest uptick in adoption during the 2020/21 period due to the pandemic. Currently, digital payment data is not analyzed specifically under the vulnerable (elder and dependent adult) financial exploitation lens. Banks are required to report elder financial abuse but, unless a customer reports fraud and files a claim, financial abuse can go undetected and repeated fraud via digital payments can continue without the banks’ knowledge. Without detection models, a large amount of fraud is left unreported by consumers and elder and vulnerable adult populations will be at greater risk of being targeted and losing savings to fraudulent payments.

Banks need better methods to help protect elder and vulnerable adults against fraud in the digital payments landscape. Predictive modeling may also be applied in some form to alert consumers and bankers in advance of a fraud attempt and potentially pre-empt certain transactions and monetary losses. As the older adult segment continues to adopt digital technology, including digital payments, banks need better ways to predict and analyze transaction data to detect high risk payment patterns or transaction attributes that signal high risk for fraud, especially for older and vulnerable adult customers, which could be targeted by scammers.

# Data Description -
This data was provided by Wells Fargo Campus Analytics Challenge conducted by mindsumo
https://www.mindsumo.com/contests/campus-analytics-challenge-2021 

# Skills used -
- Programming Language - Python (sklearn, pandas, numpy)
- Data Science Skills - Preprocessing, Handling missing values, EDA, KNN Classifier, Logistic Regression Classifier, SVM, Decision Tree, Random Forest
-
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import sklearn
from sklearn.metrics import confusion_matrix,plot_confusion_matrix
from pathlib import Path

#Conclusion :
We get maximun roc_auc_score: 0.9694 by using Decision Tree Classifier with 'max_depth': 5, 'min_samples_leaf': 90, 'min_samples_split': 250. Also from Auc_roc curves we observe that the decision tree curve is close to top left as comparared to other models. This also proves that area under the curve, AUC is higher for the Decision Tree Classifier. Hence this is the best model to predict suspected elder fraud in the digital payments space.

