# Credit_Risk_Analysis
## Introduction
This analysis is to use data preparation, statistical reasoning, and machine learning to test credit risk on loans. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I’ll employ different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
## Results

### Random Over Sampler
![Random Over Sampler](https://user-images.githubusercontent.com/56700719/164787557-34a7b03c-af55-4801-b838-dc56fdde9e1c.JPG)
- Balanced Accuracy Score: 0.6249984891886339
- Precision(avg/total): 0.99
- Recall(avg/total): 0.65

### SMOTE
![SMOTE](https://user-images.githubusercontent.com/56700719/164787709-d60f192b-5507-4047-a779-b6171a713dab.JPG)
- Balanced Accuracy Score: 0.6512584051472337
- Precision(avg/total): 0.99
- Recall(avg/total): 0.66

### Cluster Centroids
![Cluster Centroids](https://user-images.githubusercontent.com/56700719/164787832-f31a6846-596b-4f46-adb3-c3e0162d5bbd.JPG)
- Balanced Accuracy Score: 0.5103309281216384
- Precision(avg/total): 0.99
- Recall(avg/total): 0.44

### SMOTEENN
![SMOTEENN](https://user-images.githubusercontent.com/56700719/164787917-3137b277-1d7f-4b33-bf52-2bae53065a8a.JPG)
- Balanced Accuracy Score: 0.6400726134353378
- Precision(avg/total): 0.99
- Recall(avg/total): 0.44

### Balanced Random Forest Classifier
![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/56700719/164788007-675b2f42-a6eb-4370-84f7-31582259aed0.JPG)
- Balanced Accuracy Score: 0.7885466545953005
- Precision(avg/total): 0.99
- Recall(avg/total): 0.87

### Easy Ensemble Classifier
![Easy Ensemble Classifier](https://user-images.githubusercontent.com/56700719/164788087-6d08b9a9-03f7-4167-a588-f17bf6cf91f0.JPG)
- Balanced Accuracy Score: 0.9316600714093861
- Precision(avg/total): 0.99
- Recall(avg/total): 0.94

## Summary
To summarize this analysis, using machine learning to accurately predict credit is high risk is not precise enough to be used. The Easy Ensemble Classifier had the highest scores and accuracy out of the 6-machine learning libraries, but it stilled had low precision and f1 score for high-risk which would cause a lot of low-risk credits to be falsely detected as high risk. I would not recommend any of these machine learning libraries because there still too much of a risk with not enough accuracy in predicting which credit would be high risk.
