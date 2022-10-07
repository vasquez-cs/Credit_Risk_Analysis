# Credit Risk Analysis

## Overview of the loan prediction risk analysis:

Jill has asked us to apply machine learning to solve a real-world challenge of credit card risk.

As credit risk is an inherently unbalanced classification problem, we have used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we've oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we have used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 

Finally we compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Following our analysis of the six models, we have decided that there are _ models that accurately predict credit risk.

## Results:

### RandomOverSampler
  * Balanced accuracy score
  * 
<img src="https://user-images.githubusercontent.com/107224632/194457305-9960c707-3c97-44cf-8435-e787aa470394.png" width=60% height=60%><br />
*Figure 1a: RandomOverSampler Balanced accuracy score* 

  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  
    
<img src="https://user-images.githubusercontent.com/107224632/194457476-bd04ba43-3da5-4c96-ae84-a28d935bdd5d.png" width=60% height=60%><br />
*Figure 1b: RandomOverSampler imbalanced classification report* 

### SMOTE

  * Balanced accuracy score
  
<img src="https://user-images.githubusercontent.com/107224632/194458313-98fa523b-bd4f-4c6e-a5a7-c76cf7ca52d4.png" width=60% height=60%><br />
*Figure 2a: SMOTE Balanced accuracy score* 
  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  

<img src="https://user-images.githubusercontent.com/107224632/194458346-9b4fc501-445b-482e-a677-896a36d62ee0.png" width=60% height=60%><br />
*Figure 2b: SMOTE imbalanced classification report* 

### ClusterCentroids
  * Balanced accuracy score

<img src="https://user-images.githubusercontent.com/107224632/194459416-13a68f3c-c172-4749-bb34-4eae4c8a4f02.png" width=60% height=60%><br />
*Figure 3a: ClusterCentroids Balanced accuracy score*

  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.61  

<img src="https://user-images.githubusercontent.com/107224632/194458510-782af651-2008-4c4c-a15f-49f56eddb6ef.png" width=60% height=60%><br />
*Figure 3b: ClusterCentroids imbalanced classification report* 

### over- and undersampling using the SMOTEENN algorithm
  * Balanced accuracy score

<img src="https://user-images.githubusercontent.com/107224632/194458646-98b45510-52b0-464b-af3e-4c1ce08c892c.png" width=60% height=60%><br />
*Figure 4a: SMOTEENN Balanced accuracy score*

  * High Risk precision score
    * 0.01 
  * High Risk recall score
    * 0.62  

<img src="https://user-images.githubusercontent.com/107224632/194458729-3ac8f4c6-d394-44cc-8fe5-5fff8a637ff6.png" width=60% height=60%><br />
*Figure 4b: SMOTEENN imbalanced classification report* 

### BalancedRandomForestClassifier
  * Balanced accuracy score

<img src="https://user-images.githubusercontent.com/107224632/194458935-7c79504e-a4cf-43cf-8616-197f4b46c3ff.png" width=60% height=60%><br />
*Figure 6a: BalancedRandomForestClassifier Balanced accuracy score*

  * High Risk precision score
    * 0.03 
  * High Risk recall score
    * 0.70

<img src="https://user-images.githubusercontent.com/107224632/194459064-c693f725-3961-4896-83f7-8af9de87fc24.png" width=60% height=60%><br />
*Figure 6b: BalancedRandomForestClassifier imbalanced classification report* 

### EasyEnsembleClassifier
  * Balanced accuracy score

<img src="https://user-images.githubusercontent.com/107224632/194459180-b38c7d81-d6c3-4ae7-b1dc-9af8b328d208.png" width=60% height=60%><br />
*Figure 6a: EasyEnsembleClassifier Balanced accuracy score* 

  * High Risk precision score
    * 0.03 
  * High Risk recall score
    * 0.70

<img src="https://user-images.githubusercontent.com/107224632/194459228-db3a3583-3bb9-4220-abac-c986981313f3.png" width=60% height=60%><br />
*Figure 6b: EasyEnsembleClassifier imbalanced classification report* 

## Summary:

Following our analysis of the six models, the recommendation is to use the model to use the BalancedRandomForestClassifier() and the EasyEnsembleClassifier().

The two recommended models have a balance accuracy score of 0.79, which is pretty solid considering the unbalanced classification problem of identifying high risk loans. Along those lines, we were informed that "good loans easily outnumber risky loans". Therefore using these two models are recommended because they have a precision score highest amongst the models and high recall scores for high risk loans. Since high risk loans are going to be lower than good or low risk loans, we would expect a low precision for the high risk vs low risk loans. At 0.3, its not the best, but the best amongst the models for classifying high risk loans. Finally our recall is at 0.70, which means the models are accurately classifying most of the high risk loans that they are classifying.

