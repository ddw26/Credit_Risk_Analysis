# Credit_Risk_Analysis

# Overview 
Now is the time to tackle the real-world problem of credit risk. LendingClub offers peer-to-peer lending services to its customers, and aims to utilize machine learning on existing datasets to determine the risk associated with new applications. Due to the unbalanced classification problem inherent with credit risk, good loans easily outnumber risky loans. Therefore, I am tasked with employing different techniques to train models with unbalanced classes (scikit-learn and imbalanced-learn), evaluating the performance of said models, and offering recommendions on whether the models should be used to predict credit risk.


# Analysis & Results: 

### Naive Random Oversampling
Type | Score Results
Balanced accuracy score | 65.3%
Precision score | 99%
Precision score (high_risk)| 1%
Precision score (low_risk)| 100%
Recall score (avg / total)| 67%
Recall score (high_risk)| 63%
Recall score (low_risk)| 67%


![Naive Random Oversampling](https://user-images.githubusercontent.com/77905862/130278869-89ad5a41-9538-4155-9e6f-4baa2316425e.png)

### SMOTE Oversampling

![SMOTE ](https://user-images.githubusercontent.com/77905862/130279060-df1a86e0-8a6d-4174-8972-f908fd94ebfc.png)

### Undersampling

![Undersampling](https://user-images.githubusercontent.com/77905862/130279211-184369f2-d49b-474b-b654-ce96a2802242.png)

### Combined Over + Undersampling

![Over and Under](https://user-images.githubusercontent.com/77905862/130279369-45edfdf9-7a50-4a4b-a4f3-035d1995b58f.png)


## Recommendations: 
