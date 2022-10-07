Credit_Risk_Analysis
## Overview of the loan prediction risk analysis:

Jill has asked us to apply machine learning to solve a real-world challenge of credit card risk.

As credit risk is an inherently unbalanced classification problem, we have used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we've oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we have used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 

Finally we compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Following our analysis of the six models, we have decided that there are _ models that accurately predict credit risk.

### Results:

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)
Summary:

There is a summary of the results (2 pt)

There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
