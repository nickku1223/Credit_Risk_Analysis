# Credit_Risk_Analysis

# Overview of the project:
The credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans, as the dataset we use in this project. So we will need to use different techniques to train and evalute models with unbalanced classes. In this project, we will use a few different different models including RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN algorithms and compare the results.

We will also use two other machine learning models, BalanceRandomForestClassifier and EasyEnsembleClassifier to reduce bias and predict the credit resk.

# Results
- First, I try the logistic regression classifier model without modifying the sample:  
  Accuracy score: 0.99  
  Precision: high_risk: 0.81, low_risk: 1.00  
  Recall: high_risk: 0.21, low_risk: 1.00  
  F1 score: high_risk: 0.33, low_risk: 1.00  
  
- Oversampling with RandomOverSampler:  
  Balanced Accuracy Score: 0.84  
  Precision: high_risk: 0.03, low_risk: 1.00  
  Recall: high_risk: 0.82, low_risk: 0.84  
  F1 score: high_risk: 0.06, low_risk: 0.91  
  
- Oversampling with SMOTE:  
  Balanced Accuracy Score: 0.87  
  Precision: high_risk: 0.04, low_risk: 1.00  
  Recall: high_risk: 0.82, low_risk: 0.87  
  F1 score: high_risk: 0.07, low_risk: 0.93  
  
- Undrsampling with ClusterCentroids:  
  Balanced Accuracy Score: 0.76  
  Precision: high_risk: 0.02, low_risk: 1.00  
  Recall: high_risk: 0.88, low_risk: 0.76  
  F1 score: high_risk: 0.04, low_risk: 0.86  
  
  ![Scores 1](Images/deliverable_1_score.png)
  
- Combination sampling with SMOTEENN:  
  Balanced Accuracy Score: 0.84  
  Precision: high_risk: 0.03, low_risk: 1.00  
  Recall: high_risk: 0.83, low_risk: 0.86 
  F1 score: high_risk: 0.06, low_risk: 0.92  
  
  ![Scores 2](Images/deliverable_2_score.png)

- With BalancedRandomForestClassifier:
  Balanced Accuracy Score: 0.75  
  Precision: high_risk: 0.03, low_risk: 1.00  
  Recall: high_risk: 0.63, low_risk: 0.88 
  F1 score: high_risk: 0.06, low_risk: 0.94
  
  ![Scores 3](Images/deliverable_3_1_score.png)
  
- With EasyEnsembleClassifier:
  Balanced Accuracy Score: 0.93  
  Precision: high_risk: 0.09, low_risk: 1.00  
  Recall: high_risk: 0.92, low_risk: 0.94 
  F1 score: high_risk: 0.16, low_risk: 0.97
  
  ![Scores 3](Images/deliverable_3_2_score.png)  
