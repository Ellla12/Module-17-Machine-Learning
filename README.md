# Module 17: Machine-Learning

## Overview:

The purpose of the analysis is to build and evaluate several machine learning models to predict credit risk. For this challenge, we are tasked with the following:

- use imbalanced-learn and scikit-learn libraries build and evaluate models using resampling
- from the sampling, use the data to predict credit risk

## Results:

### Results for credit_risk_resampling:

1. Balanced Accuracy Score
- The Naive Random Oversampling: `0.65709630773648`
- SMOTE Oversampling: `0.6536039858663134`
- Undersampling: `0.5441784794709592`
- Combination (Over and Under) Sampling: `0.6419727537533921`

Naive Random Oversampling has the best  balanced accuracy  score with undersampling being the worst one.

2. Precision Score AVG
- The Naive Random Oversampling: `0.99`
- SMOTE Oversampling: `0.99`
- Undersampling: `0.99`
- Combination (Over and Under) Sampling: `0.99`

All 4 methods have the same precision average score.

3. Recall Score AVG
- The Naive Random Oversampling: `0.60`
- SMOTE Oversampling: `0.69`
- Undersampling: `0.40`
- Combination (Over and Under) Sampling: `0.58`

Despite Naive Random Oversampling having the best balanced accuracy score, SMOTE oversampling has the best recall score.

### Results for credit_risk_ensemble:

1. Balanced Accuracy Score
- Balanced Random Forest Classifier: `0.7885466545953005`
- Easy Ensemble AdaBoost Classifier: `0.9316600714093861`

Easy Ensemble is the better sampling method, as it has a better Balanced Accuracy Score.

2. Precision Score
- Balanced Random Forest Classifier: `0.99`
- Easy Ensemble AdaBoost Classifier: `0.99`
Both methods have the same precision average score.

3. Recall Score
- Balanced Random Forest Classifier: `0.87`
- Easy Ensemble AdaBoost Classifier: `0.94`

With the recall score, it further shows that Easy Ensemble is the better method.

## Summary:
From the results, we can conclude that for credit_risk_resampling the best method to use is either Naive Random Oversampling or SMOTE Oversampling. For credit_risk_ensemble, we can conclude that Easy Ensemble Adaboost Classifier is the better method to use.