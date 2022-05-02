# Credit Risk Analysis

## Overview

To better determine potential customers' credit risk, we employee several Supervised Machine Learning Algorithms to determine if there is a model that does a decent job of predicting credit risk.  We first utilize three methods of sampling algorithms and use logistic regression to make predictions to evaluate the models.  Second, we utilize an over and undersampling method called SMOTEENN. Finally, we use two Ensamble Classifiers.  For all these methods, we calculate the balanced accuracy score, create the confusion matrix, and generate a classification report so we can evaluate each and compare effectiveness in determining credit risk across all models.

## Results

The results of the six different learning models are displayed below for easy comparison.  Following the chart, you'll find the individual results captured for each of these metrics. 

![Model Comparison Chart](images/ModelComparisonChart.PNG)

* Naive Random Sampling - Balance Accuracy Score & Imbalanced Classification Chart

![Naive Random Oversampler Balance Accuracy Score](images/NaiveRandomOversampler-BAC.PNG)
![Naive Random Oversampler Imbalance](images/NaiveRandomOversampler-ICR.PNG)

* SMOTE - Balance Accuracy Score & Imbalanced Classification Chart

![SMOTE Balance Accuracy Score](images/SMOTE-BAC.PNG)
![SMOTE Imbalance](images/SMOTE-ICR.PNG)

* Cluster Centroids - Balance Accuracy Score & Imbalanced Classification Chart

![Cluster Centroids Balance Accuracy Score](images/ClusterCentroids-BAC.PNG)
![Cluster Centroids Imbalance](images/ClusterCentroids-ICR.PNG)

* SMOTEENN - Balance Accuracy Score & Imbalanced Classification Chart

![SMOTEENN Balance Accuracy Score](images/SMOTEENN-BAS.PNG)
![SMOTEENN Imbalance](images/SMOTEENN-ICR.PNG)

* Balanced Random Forest Classifier - Balance Accuracy Score & Imbalanced Classification Chart

![BalancedRandomForestClassifier Balance Accuracy Score](images/BalancedRandomForestClassifier-BAS.PNG)
![BalancedRandomForestClassifier Imbalance](images/BalancedRandomForestClassifier-ICR.PNG)

* Easy Ensemble Classifier - Balance Accuracy Score & Imbalanced Classification Chart

![EasyEnsembleClassifier Balance Accuracy Score](images/EaseEnsembleClassifier-BAS.PNG)
![EasyEnsembleClassifier Imbalance](images/EaseEnsembleClassifier-ICR.PNG)


Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
