# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.
  - The purpose of this analysis is to apply machine learning to solve a real-world challenge, credit card risk, by using imbalanced-learn and scikit-learn libraries to build and  evaluate models using resampling.
  - Additionally, to predict credit risk, I used RandomOverSampler and SMOTE for oversampling data.  ClusterCentroids and SMOTEENN were used for undersampling dataset. Lastly, I used new machine learning models   which are BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

  ## Oversampling
   •	The sensitivity/recall score for high risk loans is 73%, meaning that most of the loans defined as high risk were identified as such, but we may have missed identifying 27% of loans as high risk, meaning they were false negative.  On the other hand, 57% of low risk loans were low risk, but we may have missed identifying 43% of loans as low risk, meaning 43% were false negative for low risk.
   •	The precision/specificity of high risk loans was only 1%.  This indicates that we may have incorrectly identified 99% of high risk loans as high risk, as they may be false positives.  On the other hand, the low risk loan precision/specificity was nearly 100%, meaning that these low risk loans were correctly identified as low risk, leaving little to zero chance of a loan being incorrectly identified as low risk (false positive).
   •	Total balanced accuracy score for RandomeOverSampler algorithm is 65%.
   
   ![image](https://user-images.githubusercontent.com/83877498/133012084-08f6ea40-d625-486b-a6d0-02d91168c98d.png)

   •	The sensitivity/recall score for high risk loans is 63%, meaning that most of the loans defined as high risk were identified as such, but we may have missed identifying 37% of loans as high risk, meaning they were false negative.  On the other hand, 68% of low risk loans were low risk, but we may have missed identifying 32% of loans as low risk.
   •	The precision/specificity of high risk loans was only 1%.  This indicates that we may have incorrectly identified 99% of high risk loans as high risk, as they may be false positives.  On the other hand, the low risk loan precision/specificity was nearly 100%, meaning that these low risk loans were correctly identified as low risk, leaving little to zero chance of a loan being incorrectly identified as low risk (false positive).
   •	Total balanced accuracy score for SMOTE algorithm is 66%.
   
   ![image](https://user-images.githubusercontent.com/83877498/133012111-0b7aecdb-5d1a-486d-b783-63f88b046ca7.png)

## Undersampling

   •	The sensitivity/recall score for high risk loans is 69%, meaning that most of the loans defined as high risk were identified.  On the other hand, 39% of low risk loans were  low risk, but we may have missed identifying 61% of loans as low risk.
   •	The precision/specificity of high risk loans was only 1%.  This indicates that we may have incorrectly identified 99% of high risk loans as high risk, as they may be false positives.  On the other hand, the low risk loan precision/specificity was nearly 100%, meaning that these low risk loans were correctly identified as low risk, leaving little to zero chance of a loan being incorrectly identified as low risk (false positive).
   •	Total balanced accuracy score for ClusterCentroids algorithm is 54%.
   
   ![image](https://user-images.githubusercontent.com/83877498/133012147-5d06ee96-45fc-412f-896a-00c7d1c6dede.png)


   •	The sensitivity/recall score for high risk loans is 72%, meaning that most of the loans defined as high risk were identified.  On the other hand, 58% of low risk loans were low risk, but we may have missed identifying 42% of loans as low risk.
   •	The precision/specificity of high risk loans was only 1%.  This indicates that we may have incorrectly identified 99% of high risk loans as high risk, as they may be false positives.  On the other hand, the low risk loan precision/specificity was nearly 100%, meaning that these low risk loans were correctly identified as low risk, leaving little to zero chance of a loan being incorrectly identified as low risk (false positive).
   •	Total balanced accuracy score for SMOTEENN method is 65%.

  ![image](https://user-images.githubusercontent.com/83877498/133012189-bd4232d5-c6a5-4793-a8ed-66837adcaa0b.png)


  ## Balanced Random Forest Classifier
  
  •	The sensitivity/recall score for high risk loans is 68%, meaning that most of the loans defined as high risk were identified.  On the other hand, 88% of low risk loans were low risk and only 12% may have missed identifying low risk loans.
  •	The precision/specificity of high risk loans was only 3%.  This indicates that we may have incorrectly identified 99% of high risk loans as high risk, as they may be false positives.  On the other hand, the low risk loan precision/specificity was nearly 100%, meaning that these low risk loans were correctly identified as low risk, leaving little to zero chance of a loan being incorrectly identified as low risk (false positive).
  •	Total balanced accuracy score for SMOTEENN method is 78%.
  
  ![image](https://user-images.githubusercontent.com/83877498/133012238-db8c95b7-72be-4872-bcc4-a7a75e65cb69.png)

## Easy Ensemble AdaBoost Classifier

  •	The sensitivity/recall score for high risk loans is 92%, meaning that most of the loans defined as high risk were identified.  On the other hand, 94% of low risk loans were low risk and only 6% may have missed identifying low risk loans.
  •	The precision/specificity of high risk loans was only 9%.  This indicates that we may have incorrectly identified 99% of high risk loans as high risk, as they may be false positives.  On the other hand, the low risk loan precision/specificity was nearly 100%, meaning that these low risk loans were correctly identified as low risk, leaving little to zero chance of a loan being incorrectly identified as low risk (false positive).
  •	Total balanced accuracy score for SMOTEENN method is 78%.
  
  ![image](https://user-images.githubusercontent.com/83877498/133012278-89dd92b6-38c4-4fb1-b6ec-22fcf1044a76.png)

## 3.	Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

  •	Based on the result of the analysis, Balanced Random Forest Classifier and Early EnsembleClassifier are effective in identifying predictions of credit risk for the loan status. 
  •	Both can be used on a wide range of problems that's used to solve regression and classification problems, however, performance of the standard algorithm is not great on imbalanced classification problem.
  •	I think I would recommend using Early EnsembleClassifier for this kind of dataset because of the results of the recall as well the higher percentage of balance accuracy score. This would show that incorrectly identified credit risk is lower and it would have less impact.


  



  
   



