# Credit Risk Analysis

# Overview of the analysis

The purpose of this analysis is to create a machine learning model that can accurately identify loan applicants as high or low risk.

The challenge unique to this dataset is the occurance of high risk loan applicants is very low. This makes it difficult for any model to accurately predict and identify high risk applicants. 

To overcome this issue, 4 different sampling methods and 2 ensemble are applied to the modeling.

Throughout the analysis the following values are used to identify a loan applicants status:

0 = high risk,
1 = low risk

# Results

## Balanced Accuracy

### Sampling Methods

![Sampling](./resources/accuracy_sample.PNG)

Of the sampling strategies, both SMOTE and SMOTEENN performed the best.

### Ensemble Methods

![Ensemble](./resources/accuracy_ensemble.PNG)

Of the ensemble methods, Easy Ensemble Classifier performed the best.

## Classification Reports

### Oversampling
![Over](./resources/over.PNG)

### SMOTE 

![SMOTE](./resources/SMOTE.PNG)

### Undersampling

![Under](./resources/under.PNG)

### SMOTEENN

![SMOTEENN](./resources/SMOTEENN.PNG)

### Balanced Random Forest Classifier

![BRFC](./resources/brfc.PNG)

### Easy Ensemble Classifier

![EEC](./resources/eec.PNG)

# Summary

The three best performing models by balanced accuracy are SMOTE, SMOTEENN, and Easy Ensemble Classifier. Of these three, SMOTE and SMOTEENN have F1 scores in high risk detection of 0.06 and 0.05 respectfully.

Both the SMOTE and SMOTEENN have senstivities of 0.71 and 0.72 for high risk. Given that high risk loan applicants are rare, these models could be useful. A review of their confusion matrices provides further details about their performance.

## SMOTE

## SMOTEENN