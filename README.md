# Credit_Risk_Analysis

## Overview of Analysis 
### Purpose:
The purpose of this analysis was to use the dataset from LendingClub to oversample and undersample the data utlizing oversampling, undersampling and combinational machine learning models in order to determine which model should be used to predict credit risk. 
## Results
### Naive Random oversampling
![random_oversampler](https://github.com/Cmarescot/Credit_Risk_Analysis/blob/main/images/random_oversampler.png)
- Balanced accuracy score: The model has a relatively low  accuracy of 0.646.
- Precision: There was a Precision score of 0.01 for high risk and 1.00 for low risk. This means that the model does a great job at accurately predicting low credit risk but not high credit risk. Of the 5496 classified as high credit card risks 5442 were actually low credit card risks. Meaning a lot of people were predicted as having being high credit risks when in reality they were low credit risks. 
- Recall: The model had a recall (or sensitivity) of 0.61 for high risk and 0.68 for low risk. This means that the model doesnt really do a good job at finding all the high and low credit risk.
 
### SMOTE oversampling
![smote](https://github.com/Cmarescot/Credit_Risk_Analysis/blob/main/images/smote.png)
- Balanced accuracy score: The model had a low accuracy of 0.623.
- Precision: There was a Precision score of 0.01 for high risk and 1.00 for low risk. This means that the model does a great job at accurately predicting low credit risk but not high credit risk. Of the 6255 classified as high credit card risks 6193 were actually low credit card risks. Meaning a lot of people were predicted as having being high credit risks when in reality they were low credit risks.
- Recall: The model had a recall (or sensitvity) of 0.61 for high risk and 0.64 for low risk. This means that the model doesnt really do a good job at finding all the high and low credit risk.
### Undersampling 
![cluster_centroids](https://github.com/Cmarescot/Credit_Risk_Analysis/blob/main/images/cluster_centroids).png)
- Balanced accuracy score: The model has a very low accuracy 0.519.
- Precision: There was a Precision score of 0.01 for high risk and 1.00 for low risk. This means that the model does a great job at accurately predicting low credit risk but not high credit risk. Of the 9199 classified as high credit card risks 9108 were actually low credit card risks. Meaning a lot of people were predicted as having being high credit risks when in reality they were low credit risks.
- Recall: The model had a recall (or sensitvity) of 0.57 for high risk 0.46 for low risk. This means that the model doesnt do a good job at finding all the high and low credit risk.
### Combination (over and under) Sampling 
![smoteen](https://github.com/Cmarescot/Credit_Risk_Analysis/blob/main/images/smoteen.png)
- Balanced accuracy score: The model has a low accuracy 0.639.
- Precision: There was a Precision score of 0.01 for high risk and 1.00 for low risk. This means that the model does a great job at accurately predicting low credit risk but not high credit risk. Of the 7285 classified as high credit card risks 7213 were actually low credit card risks. Meaning a lot of people were predicted as having being high credit risks when in reality they were low credit risks.
- Recall: The model had a recall  (or sensitvity) of 0.70 for high risk and .58 for low risk. This means that the model does an okay job at finding all the high credit risks but does a bad job at finding the low credit risks.
### Balanced Forest Learner Classifier 
![balanced_random_forest](https://github.com/Cmarescot/Credit_Risk_Analysis/blob/main/images/balanced_random_forest.png)
- Balanced accuracy score: The model has a decent accuracy score of 0.788.
- Precision: There was a Precision score of 0.04 for high risk and 1.00 for low risk. This means that the model does a great job at accurately predicting low credit risk but not high credit risk. Of the 1618 classified as high credit card risks 1554 were actually low credit card risks. Meaning a lot of people were predicted as having being high credit risks when in reality they were low credit risks.
- Recall: The model had a recall (or sensitivity) of 0.67 for high risk and 0.91 for low risk. This means that the model doesnt really do a good job at finding all of the high credit card risks but does a good job at finding all the low credit card risks. 
### Easy Ensemble AdaBoost Classifier 
![easy_ensemble_classifier](https://github.com/Cmarescot/Credit_Risk_Analysis/blob/main/images/easy_ensemble_classifier.png)
- Balanced accuracy score: The model has a high accuracy score of 0.925.
- Precision: There was a Precision score of 0.07 for high risk and 1.00 for low risk. This means that the model does a great job at accurately predicting low credit risk but not high credit risk. Of the 1058 classified as high credit card risks 984 were actually low credit card risks. Meaning a lot of people were predicted as having being high credit risks when in reality they were low credit risks.
- Recall:The model had a recall score of 0.91 for high risk and 0.94 for low risk. Which means that the model does a good job at finding the positive high and low credit risks. 
## Summary
### Accuracy score
Of all the machine learning models the Easy Ensemble Adaboost Classifier has the highest accuracy score of 0.925, followed by Balanced Forest Learning Classifier which has a score of 0.788. 
### Precison 
The Precision scores throughout all of the models were relatively the same with the models doing a great job at accurately predicting low credit risks but not high credit risks. In this instance having a low precison score for high credit risk isnt so bad because companies would rather have false positives than false negatives. 
### Recall 
The Easy Ensemble AdaBoost Classifier has the highest recal/sensitivity scores of 0.91 for high risk and 0.94 for low risk. This means that overall the model does a good job at finding all the postive samples. 
### Recommendations 
Based on the results, I would recommend using the Easy Ensemble Adaboost Classifier because it has the highest accuracy score and the highest sensitivity score.
