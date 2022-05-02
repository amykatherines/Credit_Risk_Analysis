# Credit Risk Analysis

## Overview

To better determine potential customers' credit risk, we employee several Supervised Machine Learning Algorithms to determine if there is a model that does a decent job of predicting credit risk.  We first utilize three methods of sampling algorithms and use logistic regression to make predictions to evaluate the models.  Second, we utilize an over and undersampling method called SMOTEENN. Finally, we use two Ensemble Classifiers.  For all these methods, we calculate the balanced accuracy score, create the confusion matrix, and generate a classification report so we can evaluate each and compare effectiveness in determining credit risk across all models.

## Results

The results of the six different learning models are displayed below for easy comparison.  To determine the best option in the learning models, we focused in on the Balance Accuracy Score, Precision, Recall/Sensitivity, and F1 scores.  Following the chart, you'll find the individual results captured for each of these metrics. 

![Model Comparison Chart](images/ModelComparisonChart.PNG)

* Naive Random Sampling - The Accuracy score for this model is not good at .67, we want it to be closer to 1.0. Coupled with the very low precision of .01, only so-so precision at .71 and a very low F1 score, this model is not a good fit for identifying high risk customers. 

![Naive Random Oversampler Balance Accuracy Score](images/NaiveRandomOversampler-BAC.PNG)
![Naive Random Oversampler Imbalance](images/NaiveRandomOversampler-ICR.PNG)

* SMOTE - This Sampling method resulted in similar scores as the Random Sampling method with even lower scores for the balance accuracy score and recall.  It is not a good fit for our dataset.

![SMOTE Balance Accuracy Score](images/SMOTE-BAC.PNG)
![SMOTE Imbalance](images/SMOTE-ICR.PNG)

* Cluster Centroids -  This sampling method is also not a good fit with low scores similar to the previous other sampling methods.

![Cluster Centroids Balance Accuracy Score](images/ClusterCentroids-BAC.PNG)
![Cluster Centroids Imbalance](images/ClusterCentroids-ICR.PNG)

* SMOTEENN - This method uses a combination of over and under-sampling to evaluate the data.  The test shows that it too falls short in the key scores that would indicate a good fit.

![SMOTEENN Balance Accuracy Score](images/SMOTEENN-BAS.PNG)
![SMOTEENN Imbalance](images/SMOTEENN-ICR.PNG)

* Balanced Random Forest Classifier - This forest classification method had a slightly better balance accuracy score at .78 but the other metrics fall short like the previous sampling methods.

![BalancedRandomForestClassifier Balance Accuracy Score](images/BalancedRandomForestClassifier-BAS.PNG)
![BalancedRandomForestClassifier Imbalance](images/BalancedRandomForestClassifier-ICR.PNG)

* Easy Ensemble Classifier - The Adaptive Boosting method of Machine Learning resulted in the best scores.  The balance accuracy score was the closest to 1 at .929.  All the other metrics were improved over all the previous tests with Sensitivity at a .92.  The precision of the model is low at .07 but because the Sensitivity is high, we know there is usually a trade-off with precision.  The F1 score is still not great but expected because there's a pronounced imbalance between sensitivity and precision.

![EasyEnsembleClassifier Balance Accuracy Score](images/EaseEnsembleClassifier-BAS.PNG)
![EasyEnsembleClassifier Imbalance](images/EaseEnsembleClassifier-ICR.PNG)

## Summary

In summary, we found that the Boosting Machine Learning model AdaBoost produced the best scores for balanced accuracy and sensitivity/recall. The precision was very low so there are a lot of records flagged as High Risk which were not high-risk. We think the trade-off is worth it though, since a customer flagged as possibly high-risk can be further analyzed in other ways specific to the individual case and moved to low-risk following other analysis.  
