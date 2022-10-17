# Credit_Risk_Analysis

## Overview
In this project, we implemented 6 different supervised machine learning techniques to train and evaluate credit risk. Credit risk is a clear example of a classification scenario, where their are discrete outcomes which can be answered in a "yes" or "no". Credit risk is also considered to have an uneven or imbalanced distribution because it's very likely one class is significantly bigger than other, in this case the number of good loanees is much smaller than the number of bad loanees.<br/>

We used the following models to produce the best quality results in determining somone's credit worthiness:<br/>

- RandomOverSampler<br/>
- SMOTE<br/>
- ClusterCentroids<br/>
- SMOTEENN<br/>
- BalancedRandomForestClassifier <br/>
- EasyEnsembleClassifier<br/>

## Results

Accuracy can be subjective, so it's common practice to consider anything within the 70%-90% as a realistic machine learning model and will provide valid results. Accuracy alone doesn't tell the full story when you're working with a class-imbalanced data set, like this one, where there is a significant disparity between the number of positive and negative scores. Precision is the proportion of positive identification that were actually correct and Recall is the proportion of actual positives was identified correctly. 

![Screen Shot 2022-10-16 at 10 18 38 PM](https://user-images.githubusercontent.com/107026442/196095118-f3be1b2f-de8f-4350-b5d9-3b3ed8442f83.png)

![Screen Shot 2022-10-16 at 10 12 13 PM](https://user-images.githubusercontent.com/107026442/196094320-3abf276d-8d5e-4178-b5dd-470b5691bd7d.png)

![Screen Shot 2022-10-16 at 10 11 27 PM](https://user-images.githubusercontent.com/107026442/196094253-c9522a3f-3181-44c9-a046-317d583457eb.png)


### Naive Random Oversampling

<img width="710" alt="Screen Shot 2022-10-16 at 2 51 13 PM" src="https://user-images.githubusercontent.com/107026442/196094362-c8151919-164b-400b-89c0-55588d0e0b70.png">

- Balanced Accuracy:<br/>
    0.6368573512052247<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.60 High-risk loans<br/>
    0.68 Low-risk loans<br/>


### SMOTE Oversampling

![Screen Shot 2022-10-16 at 9 11 54 PM](https://user-images.githubusercontent.com/107026442/196094378-10d0491d-e8c2-4c7d-a69a-385b5a2f9c52.png)

- Balanced Accuracy:<br/>
    0.6320086539275053<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.60 High-risk loans<br/>
    0.67 Low-risk loans<br/>

### Undersampling

![Screen Shot 2022-10-16 at 9 13 33 PM](https://user-images.githubusercontent.com/107026442/196094392-b96d2d66-71e0-4875-840d-0b84ac12dbe3.png)

- Balanced Accuracy:<br/>
    0.6320086539275053<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.61 High-risk loans<br/>
    0.45 Low-risk loans<br/>

### Combination Under-Over Sampling

![Screen Shot 2022-10-16 at 9 15 28 PM](https://user-images.githubusercontent.com/107026442/196094407-923e2819-2a84-4b0e-949d-98a9e3cc1728.png)

- Balanced Accuracy:<br/>
    0.5293318990697431<br/>
- Precision: <br/>
    0.01 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.69 High-risk loans<br/>
    0.61 Low-risk loans<br/>

### Balanced Random Forest Classifier

![Screen Shot 2022-10-16 at 9 16 58 PM](https://user-images.githubusercontent.com/107026442/196094418-a6dca05b-781a-4d80-9614-8804243b3395.png)

- Balanced Accuracy:<br/>
    0.7877672625306695<br/>
- Precision: <br/>
    0.04 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.67 High-risk loans<br/>
    0.91 Low-risk loans<br/>

### Easy Ensemble AdaBoost Classifier

![Screen Shot 2022-10-16 at 9 18 28 PM](https://user-images.githubusercontent.com/107026442/196094437-1cacb2d6-f148-4f56-913d-101dad2556dc.png)

- Balanced Accuracy:<br/>
    0.925427358175101<br/>
- Precision: <br/>
    0.07 High-risk loans<br/>
    1.00 Low-risk loans<br/>
- Recall:<br/>
    0.91 High-risk loans<br/>
    0.94 Low-risk loans<br/>


## Summary

Easy Ensemble AdaBoost Classifier is the best model for evaluating credit risk due to its Accuracy level of 93%, recall score at .91 and .94 for high and low risk loans respectively. These were the highest metrics of all the models that were ran. 



