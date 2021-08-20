# Credit_Risk_Analysis

# Overview 
Now is the time to tackle the real-world problem of credit risk. LendingClub offers peer-to-peer lending services to its customers, and aims to utilize machine learning on existing datasets to determine the risk associated with new applications. Due to the unbalanced classification problem inherent with credit risk, good loans easily outnumber risky loans. Therefore, I am tasked with employing different techniques to train models with unbalanced classes (scikit-learn and imbalanced-learn), evaluating the performance of said models, and offering recommendions on whether the models should be used to predict credit risk.


# Results: 

### Naive Random Oversampling
Category | % Results
------------ | -------------
Balanced Accuracy Score | 64.7%
Precision Score | 99%
High Risk Precision score| 1%
Low Risk Precision score | 100%
Avg Recall Score | 60%
High RIsk Recall Score | 69%
Low Risk Recall Score | 60%



- ![Naive Random Oversampling](https://user-images.githubusercontent.com/77905862/130278869-89ad5a41-9538-4155-9e6f-4baa2316425e.png)

 ### SMOTE Oversampling
Category | % Results
------------ | -------------
Balanced Accuracy Score | 66.2%
Precision Score | 99%
High Risk Precision score| 1%
Low Risk Precision score | 100%
Avg Recall Score | 69%
High Risk Recall Score | 63%
Low Risk Recall Score | 69%



- ![SMOTE ](https://user-images.githubusercontent.com/77905862/130279060-df1a86e0-8a6d-4174-8972-f908fd94ebfc.png)

### Undersampling
Category | % Results
------------ | -------------
Balanced Accuracy Score | 66.2%
Precision Score | 99%
High Risk Precision score| 1%
Low Risk Precision score | 100%
Avg Recall Score | 69%
High Risk Recall Score | 63%
Low Risk Recall Score | 69%



- ![Undersampling](https://user-images.githubusercontent.com/77905862/130279211-184369f2-d49b-474b-b654-ce96a2802242.png)

### Combined Over + Undersampling
Category | % Results
------------ | -------------
Balanced Accuracy Score | 66.2%
Precision Score | 99%
High Risk Precision score| 1%
Low Risk Precision score | 100%
Avg Recall Score | 57%
High Risk Recall Score | 78%
Low Risk Recall Score | 57%



- ![Over and Under](https://user-images.githubusercontent.com/77905862/130279369-45edfdf9-7a50-4a4b-a4f3-035d1995b58f.png)
 
 
 --------------------------------------------------------------------------------------------------------------

### Balanced Random Forest Classifier
Category | % Results
------------ | -------------
Balanced Accuracy Score | 82.4%
Precision Score | 99%
High Risk Precision score| 4%
Low Risk Precision score | 100%
Avg Recall Score | 90%
High Risk Recall Score | 75%
Low Risk Recall Score | 90%



- ![Balanced RandomForest](https://user-images.githubusercontent.com/77905862/130282181-24b018c6-7f32-4dee-9e41-080fe9aad684.png)

### Easy Ensemble AdaBoost Classifier
Category | % Results
------------ | -------------
Balanced Accuracy Score | 94.6%
Precision Score | 99%
High Risk Precision score| 4%
Low Risk Precision score | 100%
Avg Recall Score | 90%
High Risk Recall Score | 75%
Low Risk Recall Score | 90%



- ![Easy Ensemble](https://user-images.githubusercontent.com/77905862/130282327-35c4d21e-6749-4fa0-a3ac-9dff94f5153d.png)


# Analysis & Recommendations: 

#### Analysis
As previously stated in the overview, due to an unbalanced classification inherent to credit risk data, I employed a few oversampling and undersampling models as means to guage which ones were most efficient. In the Random Forest and Ensemble AdaBoost Models the data was resampled in order to prediect the risk level of applicants in our data set. Naive Random Oversampling, SMOTE, Undersampling, and Combined Sampling all resulted in low precision scores of 0.01 in the high risk category. As for Balanced Random Forest and Easy Ensemble, the high risk precision scores fared slightly better at 0.04%.

#### Recommendations
I do not recommend LendingClub utilize oversampling and undersampling models. For the most efficient/precise models, I recommend Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier.
