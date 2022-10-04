# Credit_Risk_Analysis
## Overview of the analysis: 
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we employed different techniques to train and evaluate models with unbalanced classes. We used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once finished, we evaluated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results: 
The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores

### Naive Random Oversampling
![Screen Shot 2022-10-04 at 10 06 24 AM](https://user-images.githubusercontent.com/107209737/193882412-b7b841fa-aac5-4900-a03e-8b1de5b08138.png)

-Balance accuracy: 0.6497536370265621

-Precision: The precision is low for High-risk loans and is high for Low-risk loans.

-Recall scores: High/Low Risk (0.62/0.68)

### SMOTE Oversampling
![Screen Shot 2022-10-04 at 10 10 17 AM](https://user-images.githubusercontent.com/107209737/193883055-b3361033-be82-4391-80c8-c2f3ac62b6fb.png)

-Balance accuracy: 0.6443721269403855

-Precision: The precision is low for High-risk loans and is high for Low-risk loans.

-Recall scores: High/Low risk (0.63/0.66)

### Undersampling
![Screen Shot 2022-10-04 at 10 12 45 AM](https://user-images.githubusercontent.com/107209737/193883439-9bebdccd-5afb-443e-a84d-48cf3619f918.png)

-Balance accuracy: 0.6443721269403855

-Precision: The precision is low for High-risk loans and is high for Low-risk loans.

-Recall scores: High/Low risk (0.61/0.45)

### Combination Under-Over Sampling
![Screen Shot 2022-10-04 at 10 13 38 AM](https://user-images.githubusercontent.com/107209737/193883580-944e9b91-83b6-4b46-9b93-be375e7089e3.png)

-Balance accuracy: 0.5292734810302525

-Precision: The precision is low for High-risk loans and is high for Low-risk loans.

-Recall scores: High/Low risk (0.70/0.57)

### Balanced Random Forest Classifier
![Screen Shot 2022-10-04 at 10 14 49 AM](https://user-images.githubusercontent.com/107209737/193883771-4f54f1bc-f11b-46b0-a57c-bdfce2928633.png)

-Balance accuracy: 0.7877672625306695

-Precision: The precision is low for High-risk loans and is high for Low-risk loans.

-Recall scores: High/Low risk (0.67/0.91)

### Easy Ensemble AdaBoost Classifier
![Screen Shot 2022-10-04 at 10 16 05 AM](https://user-images.githubusercontent.com/107209737/193883993-71490f9e-602e-4e1e-87f8-354f4983c497.png)

-Balance accuracy: 0.925427358175101

-Precision: The precision is low for High-risk loans and is high for Low-risk loans.

-Recall scores:High/Low risk (0.91/0.94)

## Summary: 
When working with balanced accuracy, the highest compared accuracy closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy. The other models were below .78 balanced accuracy. For the recall score, the numbers closer to 1 would be the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score (0.91/0.94). The Easy Ensemble AdaBoost Classifier is the best machine learning model according to my analysis.
