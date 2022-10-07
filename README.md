# Credit Risk Analysis

## Overview of the loan prediction risk analysis:

Jill has asked us to apply machine learning to solve a real-world challenge of credit card risk.

As credit risk is an inherently unbalanced classification problem, we have used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we've oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we have used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 

Finally we compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Following our analysis of the six models, we have decided that there are _ models that accurately predict credit risk.

## Results:

# RandomOverSampler
![image](https://user-images.githubusercontent.com/107224632/194457305-9960c707-3c97-44cf-8435-e787aa470394.png)
*Figure 1a: RandomOverSampler Balanced accuracy score* 
  * Balanced accuracy score
![image](https://user-images.githubusercontent.com/107224632/194457476-bd04ba43-3da5-4c96-ae84-a28d935bdd5d.png)
*Figure 1b: RandomOverSampler imbalanced classification report* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  
# SMOTE
![image]()
*Figure 2a: SMOTE Balanced accuracy score* 
  * Balanced accuracy score
![image]()
*Figure 2b: SMOTE imbalanced classification report* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  
* ClusterCentroids
![image]()
*Figure 3a: ClusterCentroids Balanced accuracy score* 
  * Balanced accuracy score
![image]()
*Figure 3b: ClusterCentroids imbalanced classification report* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  
* over- and undersampling using the SMOTEENN algorithm
![image]()
*Figure 4a: SMOTEENN Balanced accuracy score* 
  * Balanced accuracy score
![image]()
*Figure 4b: SMOTEENN imbalanced classification report* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  
* BalancedRandomForestClassifier
![image]()
*Figure 5a: BalancedRandomForestClassifier Balanced accuracy score* 
  * Balanced accuracy score
![image]()
*Figure 5b: BalancedRandomForestClassifier imbalanced classification report* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  
* EasyEnsembleClassifier
![image]()
*Figure 6a: EasyEnsembleClassifier Balanced accuracy score* 
  * Balanced accuracy score
![image]()
*Figure 6b: EasyEnsembleClassifier imbalanced classification report* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62

## Summary:

ThThere is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
