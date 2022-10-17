# Credit_Risk_Analysis

## Overview
In this project we implemented different supervised machine learning techniques to train and evaluate credit risk. Credit risk clear example of a classification where their are discrete outcomes which can be answered in a "yes" or "no". Credit risk is also considered to have an uneven distribution because its very likely one class is significantly bigger than other, in this case the number of good loanees is much smaller than the number of bad loanees.<br/>

We used the following models to produce the best quality results in determining somone's credit worthiness:<br/>

- RandomOverSampler<br/>
- SMOTE<br/>
- ClusterCentroids<br/>
- SMOTEENN<br/>
- BalancedRandomForestClassifier <br/>
- EasyEnsembleClassifier<br/>

## Results

Accuracy can be subjective, so it's common practice to consider anything within the 70%-90% as a realistic machine learning model and will provide valid results. Accuracy alone doesn't tell the full story when you're working with a class-imbalanced data set, like this one, where there is a significant disparity between the number of good and bad credit loanees. Precision is the propportion of positive identification were actually correct and Recall is the proportion of actual positives was identified correctly. 

### Naive Random Oversampling
- Balanced Accuracy:<br/>
    0.6368573512052247<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.60 High-risk loans<br/>
    0.68 Low-risk loans<br/>


### SMOTE Oversampling

- Balanced Accuracy:<br/>
    0.6320086539275053<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.60 High-risk loans<br/>
    0.67 Low-risk loans<br/>

### Undersampling

- Balanced Accuracy:<br/>
    0.6320086539275053<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.61 High-risk loans<br/>
    0.45 Low-risk loans<br/>

### Combination Under-Over Sampling

- Balanced Accuracy:<br/>
    0.5293318990697431<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.69 High-risk loans<br/>
    0.61 Low-risk loans<br/>

### Balanced Random Forest Classifier

- Balanced Accuracy:<br/>
    0.7877672625306695<br/>
- Precision: <br/>
    0.04 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.67 High-risk loans<br/>
    0.91 Low-risk loans<br/>

### Easy Ensemble AdaBoost Classifier

- Balanced Accuracy:<br/>
    0.925427358175101<br/>
- Precision: <br/>
    0.07 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.91 High-risk loans<br/>
    0.94 Low-risk loans<br/>


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning. 

Easy Ensemble AdaBoost Classifier is the best model for evaluating credit risk due to its Accuracy level of 93%, recall score at .91 and .94 for high and low risk loans respectively. These were the highest metrics of all the models that were ran. 



