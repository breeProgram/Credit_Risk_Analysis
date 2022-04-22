# Credit_Risk_Analysis
##Introduction
This analysis is to use data preparation, statistical reasoning, and machine learning to test credit risk on loans. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I’ll employ different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
##Results

###Random Over Sampler
![Random Over Sampler](https://user-images.githubusercontent.com/56700719/164787557-34a7b03c-af55-4801-b838-dc56fdde9e1c.JPG)
•	Balanced Accuracy Score: 0.6249984891886339
•	Precision(avg/total): 0.99

•	Recall(avg/total): 0.65
