# Credit_Risk_Analysis

## Overview

In this project, we use Python to build and evaluate several machine learning models to predict credit risk. We applied the following ML methods: 

 - Oversampling using the RandomOverSampler and SMOTE algorithms.
 - Undersampling using the ClusterCentroids algorithm.
 - A combination approach of over-undersampling using the SMOTEENN algorithm.
 - The BalancedRandomForestClassifier algorith. 
 - The EasyEnsembleClassifier algorith. 

We will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results

### Oversampling with RandomOverSampler

![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/1.%20RandomOverSampling%201.png)
![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/1.%20RandomOverSampling%202.png)

### Oversampling with SMOTE

![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/2.%20SMOTEOverSampling%201.png)
![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/2.%20SMOTEOverSampling%202.png)

### Undersampling with ClusterCentroids

![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/3.%20UnderSampling1.png)
![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/3.%20UnderSampling2.png)

### SMOTEENN

![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/4.%20SMOTEENNsampling1.png)
![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/4.%20SMOTEENNsampling2.png)

### BalancedRandomForestClassifier

![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/5.%20BalancedRandomForrest1.png)
![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/5.%20BalancedRandomForrest2.png)

### EasyEnsembleClassifier

![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/6.%20EasyEnsembleAdaBoost1.png)
![](https://github.com/shahkibria/Credit_Risk_Analysis/blob/main/Screenshots/6.%20EasyEnsembleAdaBoost2.png)

Overall, we can see that the accuracy score for all over and undersampling methods were poor with scores ranging from the low 50 percents to the high 60 percents. using the ensable clasifiers improved the accuracy score to the high 80 percents or the low 90 percents. However, the precision of the both ensamble models remained poor leading on overall low F1 score for both. 

## Summary

The ensamble methods are much better at predicting high risk loans with accuracy in the high 80s to low 90s. However with a low precision for both models, we can see that there are a significantly high number of false positives. This means a significant number of customers are being turned down because they are being tagged as high risk even when they are not which means ultimately the bank is missing out on good customers and make a profit. Overall my recommendation would be to not use any of the 6 models used. 