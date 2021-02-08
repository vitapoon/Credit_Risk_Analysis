# Credit_Risk_Analysis

## Overview of the analysis:

In this project we want to take a look at how all the factors in our loan_stats csv help predict whether someone is low or high risk status. One method that data scientists use for this type of issue is creating a model and then evaluate and train the models that they create. In this specific project we are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first couple of models I oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. In the remaining models I used a combination approach to over and undersample the data using smoteenn. Finally, I compared two machine learning models that minimize bias, balancedrandomforestclassifier and easyensembleclassifier.

## Results:

## Naive Random Oversampling

Accuracy Score: 64%

Precision High Risk: 1%

Precision Low Risk: 100%

Recall High Risk: 66%

Recall Low Risk: 62%

## SMOTE Oversampling

Accuracy Score: 64%

Precision High Risk: 1%

Precision Low Risk: 100%

Recall High Risk: 72%

Recall Low Risk: 57%

## Cluster Centroid Undersampling

Accuracy Score: 64.4%

Precision High Risk: 1%

Precision Low Risk: 100%

Recall High Risk: 68%

Recall Low Risk: 41%

## SMOTEENN Sampling

Accuracy Score: 54.7%

Precision High Risk: 1%

Precision Low Risk: 100%

Recall High Risk: 72%

Recall Low Risk: 57%

## Balanced Random Forest Classifying

Accuracy Score: 76.4%

Precision High Risk: 30%

Precision Low Risk: 100%

Recall High Risk: 65%

Recall Low Risk: 88%

## Easy Ensemble Classifying

Accuracy Score: 93.1%

Precision High Risk: 9%

Precision Low Risk: 100%

Recall High Risk: 92%

Recall Low Risk: 94%


## Summary:

According to the models we created above, a model that lets the least amount of high risk loans pass through undetected. That correlating statistic for this is the recall rate for high risk. Looking through the different models, the ones that scored the highest was

### Easy Ensemble Classifying （92%）

Another important statistic is recall rate for low risk as it shows how many low risk loans are flagged as high risk. Looking through the different models, the ones that scored the highest was:

### Easy Ensemble Classifying （94%）

The models with the highest accuracy scores was:

### Easy Ensemble Classifying （93.1%）

After factoring in these three main statistics, the model that I would recommend to use for predicting high risk loans is the Easy Ensemble Classifying model.
