# Credit_Risk_Analysis

## Overview of the analysis
A credit risk is risk of default on a debt that may arise from a borrower failing to make required payments. In the first resort, the risk is that of the lender and includes lost principal and interest, disruption to cash flows, and increased collection costs. Therefore, it is essential for any stake holder related to a lending organisation to understand Rist and more than often its analysis. 
Similarly the investors of FAST LENDING- a peer to peer lending company wants to use Machine Learning to understand credit risk. Management believes that it will creat a better experice with Loans and borrowing. Being able to predict credit risk with machine learning algorithms can FAST LENDING predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud.

## The Analysis and its results 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we will be employing different techniques to train and evaluate models with unbalanced classes. Using the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub [LoanStats_2019Q1.csv](), a peer-to-peer lending services company, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then using a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, comparing two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, evaluating the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Analysis 

Two evaluation methods: ensemble learning and re-sampling.
The oversampling recall score (with SMOTE) has the highest score for predicting both low-risk and high risk loan statuses.
- An accuracy score for the model is calculated 
- A confusion matrix has been generated 
- An imbalanced classification report has been generated 
- The combinatorial SMOTEENN algorithm does the following:
- An accuracy score for the model is calculated 
- A confusion matrix has been generated 
- An imbalanced classification report has been generated
- We would put forward that this is the best model considering the financial cost risk associated with False Negatives. 
- The file to ReSampling : [Resampling Starter Notebook](credit_risk_resampling.ipynb)

Easy Ensemble AdaBoost Classifier performs the best with our steps & dataset. 
The EasyEnsembleClassifier algorithm does the following: 
- An accuracy score for the model is calculated 
- A confusion matrix has been generated 
- An imbalanced classification report has been generated 
- The features are sorted in descending order by feature importance 
- An accuracy score of the model is calculated 
- A confusion matrix has been generated 
- An imbalanced classification report has been generated 
- We would move forward with this estimator for further predictions.
- The File to Ensemble : [Ensemble Starter Notebook](credit_risk_ensemble.ipynb)


## Summary
Easy Ensemble AdaBoost Classifier performs the best with our steps & dataset; therefore, we would move forward with this estimator for further predictions.
The oversampling recall score (with SMOTE) has the highest score for predicting both low-risk and high risk loan statuses. We would put forward that this is the best model considering the financial cost risk associated with False Negatives.


