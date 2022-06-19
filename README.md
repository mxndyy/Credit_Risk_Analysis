# Credit_Risk_Analysis

## Analysis Overview 

The purpose of this analysis is to utilize machine learning models and evaluate the performance of the machine learning models in an effort analyze credit risk and provide Jill with your recommendations. 


## Deliverables:
This assignment consists of 3 technical analysis deliverables and a written report on the Credit Risk Analysis. 

1. ***Deliverable 1:*** Use Resampling Models to Predict Credit Risk
2. ***Deliverable 2:*** Use the SMOTEENN Algorithm to Predict Credit Risk
3. ***Deliverable 3:*** Use Ensemble Classifiers to Predict Credit Risk
4. ***Deliverable 4:*** Written Report on the Credit Risk Analysis

## Results

### Naive Random Oversampling

![naive.png](/Results/naive.png)

The balanced accuracy score is 65%. 
The high risk precision is about 1% only with 63% recall which makes a F1 only 2% only. The high number of the low risk population contributes to almost 100% precision with a recall of 67%.

### SMOTE Oversampling

![SMOTE.png](/Results/SMOTE.png)

The balanced accuracy score is 65%, similar to the model above. 
The high risk precision is about 1% only with 64% recall which makes a F1 of 2%. 
The low risk precision is almost 100% with a recall of 66%. 

### ClusterCentroids Model

![cluster_centroids.png](/Results/cluster_centroids.png)

The balanced accuracy score is 52%. 
The high risk precision is 1% with 69% recall which makes a F1 of 2%. 
Low risk sensitivity is 69%. 

### SMOTTEENN

![SMOTEEN.png](/Results/SMOTEEN.png)

The balanced accuracy score is 61%. 
The high risk precision is 1% with a 69% recall which makes a F1 of 2%
Low risk recall is 55%. 

### BalancedRandomForestClassifier 

![brfc.png](/Results/brfc.png)

The balanced accuracy score increased to 79%. 
The high risk precision is still low at 3% only with 70% recall which makes a F1 of 6%.
The low risk recall is now 90% with 100% precision. 

### Easy Ensemble AdaBoost Classifier

![easy_ensemble.png](/Results/easy_ensemble.png)

The balanced accuracy score 92%. 
The high risk precision is low 7% with 91% recall which makes a F1 of 14%. 
Low risk recall is 94% with 100% precision. 

## Summary

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. I recommend the ensemble classifiers over the first four models because typically you want a good balance of recall and precision. Easy Ensemble Classifier had the best balance of all the models because of its high accuracy score and good balance of precision and recall scores.