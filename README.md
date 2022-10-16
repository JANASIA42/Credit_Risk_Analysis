# Credit_Risk_Analysis

## Overview of the analysis 
The purpose of this analysis was to determine credit worthiness of loan applicants using machine learning (imbalanced-learn and scikit-learn libraries).
Models used included oversampling, undersampling, combination sampling.  We also used two new models that reduce bias (BalancedRandomForestClassifier and EasyEnsembleClassifier).
We looked at balance accuracy scores, along with precision and recall metrics, to see which models were the most reliable.

## Results 
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Naive Random Oversampling
Balance Accuracy: 0.629

Precision: 0.99

Recall/Sensitivity: 0.68

![image](https://user-images.githubusercontent.com/106359572/196047220-bff9074a-7e1d-48b0-b205-6705bbbd1a07.png)
![image](https://user-images.githubusercontent.com/106359572/196047258-d501f25a-307d-43bf-8f2a-a99c5976040b.png)

### SMOTE Oversampling
Balance Accuracy: 0.628

Precision: 0.99

Recall/Sensitivity: 0.63

![image](https://user-images.githubusercontent.com/106359572/196047322-6a0d1cde-33b2-416b-b97c-a5131083e257.png)
![image](https://user-images.githubusercontent.com/106359572/196047351-683bf021-8b4e-4fc4-bc83-9025ab7ac1eb.png)

### Cluster Centroids Undersampling
Balance Accuracy: 0.529

Precision: 0.99

Recall/Sensitivity: 0.45

![image](https://user-images.githubusercontent.com/106359572/196047396-a2d7176e-bdf4-4b3f-b7ab-9519b94ab13c.png)
![image](https://user-images.githubusercontent.com/106359572/196047425-bb8b3066-48a9-4057-829e-2bb0bb29cfde.png)

### SMOTEENN Combination Sampling
Balance Accuracy: 0.620

Precision: 0.99

Recall/Sensitivity: 0.54

![image](https://user-images.githubusercontent.com/106359572/196047502-97f8a22c-48c8-4c30-9d91-b8218b333613.png)
![image](https://user-images.githubusercontent.com/106359572/196047528-2a715187-4a4e-48a9-b1e8-6e5a938905fc.png)

### Balanced Random Forest Classifier
Balance Accuracy: 0.819

Precision: 0.99

Recall/Sensitivity: 0.92

![image](https://user-images.githubusercontent.com/106359572/196047583-16b2a2e0-ef37-4195-a24b-ba8bcbd0bdd1.png)
![image](https://user-images.githubusercontent.com/106359572/196047596-d3888e5d-0ed7-4aaa-9f28-21b2535eb687.png)

### Easy Ensemble AdaBoost Classifier
Balance Accuracy: 0.925

Precision: 0.99

Recall/Sensitivity: 0.94
 
![image](https://user-images.githubusercontent.com/106359572/196047635-a08a77be-a0d9-4543-ae91-cee892fbf767.png)
![image](https://user-images.githubusercontent.com/106359572/196047666-18e70a59-aea9-4566-8f50-cab9233b7843.png)


## Summary 
Based on accuracy, precision and sensitivity scores displayed above, the "easy ensemble AdaBoost classifier" model, along with the balance random forest model coming in at a close 2nd, surpassed other models in both accuracy and sensitivity by a landslide. Precision scores for all models were equal at 0.99.  
Because the purpose of this analysis was to predict potentially credit-risky borrowers, the easy ensemble model's high sensitivity score of 0.94 could be problematic in that it may drastically underestimate the percentage of credit worthy applicants.  However, with an even higher precision of 0.99, the model demonstrates its reliability in making accurate predictions.
