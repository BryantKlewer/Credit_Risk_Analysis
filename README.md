# Credit Risk Analysis

## Overview

In this analysis, variations of machine learing algorithms will be used to asses credit risk for loans given by LendingClub, a peer-to-peer lending service. Evaluations of these models will be completed to determine whether any recommendations can be made on which, if any, of the models could best predict credit risk moving forward. 

## Results

### Oversampling:
#### Naive Random Oversampling
* Balanced Accuracy: 64.39%
* Precision: High risk precision is 1% and low risk precision is 100%
* Recall: High risk recall is 69% and low risk recall is 59%
 ![naive](https://github.com/BryantKlewer/Credit_Risk_Analysis/blob/main/Images/naive_classification.png)
#### SMOTE Oversampling
* Balanced Accuracy: 66.29%
* Precision: High risk precision is 1% and low risk precision is 100%
* Recall: High risk recall is 63% and low risk recall is 69%
 ![smote_classification](https://github.com/BryantKlewer/Credit_Risk_Analysis/blob/main/Images/smote_classification.png)
### Undersampling:
#### Cluster Centroids
* Balanced Accuracy: 54.43%
* Precision: High risk precision is 1% and low risk precision is 100%
* Recall: High risk recall is 69% and low risk recall is 40%
 ![cc_classification](https://github.com/BryantKlewer/Credit_Risk_Analysis/blob/main/Images/cc_classification.png)
### Combination (Over and Under) Sampling:
#### SMOTEENN
* Balanced Accuracy: 64.48%
* Precision: High risk precision is 1% and low risk precision is 100%
* Recall: High risk recall is 72% and low risk recall is 57%
 ![smoteenn_classification](https://github.com/BryantKlewer/Credit_Risk_Analysis/blob/main/Images/smoteenn_classification.png)
### Ensemble Learners:
#### Balanced Random Forest Classifier
* Balanced Accuracy: 78.85%
* Precision: High risk precision is 3% and low risk precision is 100%
* Recall: High risk recall is 70% and low risk recall is 87%
 ![brf_classification](https://github.com/BryantKlewer/Credit_Risk_Analysis/blob/main/Images/brf_classification.png)
#### Easy Ensemble AdaBoost Classifier
* Balanced Accuracy: 93.16%
* Precision: High risk precision is 9% and low risk precision is 100%
* Recall: High risk recall is 92% and low risk recall is 94%
 ![eec_classification](https://github.com/BryantKlewer/Credit_Risk_Analysis/blob/main/Images/eec_classification.png)

## Summary

After reviewing the findings of all of the algorithms tested, it would be recommended to utilize the Easy Ensemble AdaBoost Classifier for credit decisions. The Easy Ensemble AdaBoost Classifier boasts the highest accuracy score of all the tested alorithms at 93.16%. The alorithm also produced the highest precision for high risk candidates at 9% and the highest recall for the same group at 92%. From a credit lending point of view, having this high percentage recall means that 92% of all actual high risk applicants will be flagged as high risk, this will lead to less risky loans being issued. The Easy Ensemble AdaBoost Classifier also performed extreemly well for the low risk category of applicants. Its low risk precision was 100% and recall 94%. 
