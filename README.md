# Credit_Risk_Analysis

Supervised machine learning

## OVERVIEW
  ### Purpose:  The purpose of the current analysis was to assess the performance of various algorithms/computer learning models in predicting credit risk.  Specifically, credit card data taken from LendingClub was subjected to analysis under the following algorithms and machine learning models:  RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier and EasyEnsembleClassifier.  Each model was applied to predict credit risk.  The performance of each model was then evaluated using a balanced accuracy score, confusion matrix and sensitivity (recall), precision and f1 scores.

## RESOURCES
  - Data Source: LoanStats_2019Q1.csv
  - Software:  Python 3.7.7, Anaconda, Jupyter Notebook, Pandas Library, sklearn, imblearn  

## RESULTS
  1. [RandomOverSampler](Images/RandomOverSampler.png) - The Random oversampling algorithm yielded a balanced accuracy score of 65.6%.  Precision was 0.01 for high_risk borrowers and 1.00 for low_risk borrowers.  Sensitivity(recall) was 0.69 and 0.62 for high and low_risk borrowers respectively.  The harmonic mean (f1) score was 0.02 and 0.76 for predicting high and low_risk borrowers respectively.
  
  2. [SMOTE Oversampling](Images/SMOTE.png) -  The SMOTE oversampling algorithm yielded a balanced accuracy score of 65.9%.  Precision was 0.01 for high_risk borrowers and 1.00 for low_risk borrowers.  Sensitivity(recall) was 0.63 and 0.68 for high and low_risk borrowers respectively. The harmonic mean (f1) score was 0.02 and 0.81 for predicting high and low_risk borrowers respectively.
  
  3. [ClusterCentroids Undersampling](Images/ClusterCentroids.png) - The Random oversampling algorithm yielded a balanced accuracy score of 54.4%.  Precision was 0.01 for high_risk borrowers and 1.00 for low_risk borrowers.  Sensitivity(recall) was 0.69 and 0.40 for high and low_risk borrowers respectively. The harmonic mean (f1) score was 0.01 and 0.57 for predicting high and low_risk borrowers respectively.
  
  4. [SMOTEENN Combination Over/Under sampling](Images/SMOTEENN.png) - The Random oversampling algorithm yielded a balanced accuracy score of 66.8%.  Precision was 0.01 for high_risk borrowers and 1.00 for low_risk borrowers.  Sensitivity(recall) was 0.73 and 0.60 for high and low_risk borrowers respectively. The harmonic mean (f1) score was 0.02 and 0.75 for predicting high and low_risk borrowers respectively.
  
  5. [BalancedRandomForest Classifier](Images/BalancedForest.png) - The Random oversampling algorithm yielded a balanced accuracy score of 78.8%.  Precision was 0.03 for high_risk borrowers and 1.00 for low_risk borrowers.  Sensitivity(recall) was 0.70 and 0.87 for high and low_risk borrowers respectively. The harmonic mean (f1) score was 0.06 and 0.93 for predicting high and low_risk borrowers respectively.
  
  6. [EasyEnsembleClassifier](Images/EasyEnsemble.png) - The Random oversampling algorithm yielded a balanced accuracy score of 93.2%.  Precision was 0.09 for high_risk borrowers and 1.00 for low_risk borrowers.  Sensitivity(recall) was 0.92 and 0.94 for high and low_risk borrowers respectively. The harmonic mean (f1) score was 0.16 and 0.97 for predicting high and low_risk borrowers respectively.

## SUMMARY
### From the results, we can see that several of the models struggled with predicting high_risk borrowers. Accuracy scores were overall seemingly respectable, ranging from poor (54.4%) all the way to very good (93.2%). The precision for low-risk borrowers was 1.00 for all models, however, that is not very useful.  Precision for identifying high-risk borrowers is more important, but that value was low across the board, ranging from 0.01 to 0.09 across the models.  In other words, none of the models was very precise when it comes to predicting high_risk borrowers.  In terms of Sensitivity, the EasyEnsembleClassifier scored 92%/94%, well above the other models, for both high and low_risk borrowers.  The EasyEnsembleClassifier also scored well above the other models for harmonic mean (f1) score.  Of the models tested, the EasyEnsembleClassifier definitely outperformed every other model tested. However, it can only be recommended lukewarmly, since the precision of 0.09 for predicting high-risk borrowers is still very low, as is the f1 score of 0.16 for predicting high_risk borrowers.
