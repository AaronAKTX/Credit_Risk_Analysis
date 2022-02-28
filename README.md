# Credit_Risk_Analysis

# Main Objective

 The main objective of this challenge was to build different machine learning models that can help determine credit risk. Once complete, the models were evaluated to determine if any were suitable options to use or to use as a starting place to grow from.


## Machine Learning Models

- ### OVERSAMPLING
  
  - #### RandomOverSampler algorithm<br />
Using the RandomOverSampler algorithm to resample the dataset before training the logistic regression classifier did not yield great results. Below we can see the balanced      accuracy score was 64%, the precision for high risk was was only 1% and the sensitvity for high risk  was only 62% and for low risk only 65%.
    <br /><br />
    <img src = https://github.com/AaronAKTX/Credit_Risk_Analysis/blob/main/Resources/RandomOverSampler.PNG> <br />

  - #### SMOTE algorithm  <br />
Using the SMOTE algorithm to resample the dataset before training the logistic regression classifier did also not yield very promising results. Below we can see the balanced      accuracy score was 63%, the precision for high risk was was only 1% and the sensitvity for high risk  was only 62% and for low risk only 64%.
    <br /><br />
    <img src = https://github.com/AaronAKTX/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Oversampling.PNG> <br />

- ### UNDERSAMPLING

  - #### ClusterCentroids resampling<br />
Using the CluserCentroids algorithm to undersample the dataset before training the logistic regression classifier did not prove to be a valuable prediction tool. Below we can see the balanced accuracy score was 51%, the precision for high risk was was only 1% and the sensitvity for high risk  was only 59% and for low risk only 43%.
    <br /><br />
    <img src = https://github.com/AaronAKTX/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids.PNG> <br />

- ### COMBINATION SAMPLING
  
  - #### SMOTEENN model<br />
Using the SMOTEENN algorithm to combine over and under sampling of the dataset before training the logistic regression classifier did not prove to be a valuable prediction tool. Below we can see the balanced accuracy score was 62%, the precision for high risk was was only 1% and the sensitvity for high risk was only 71% and for low risk only 54%. It is notable that of all the methods tried thus far, SMOTEENN yielded the highest sensitivity for High Risk credit accounts.
    <br /><br />
    <img src = https://github.com/AaronAKTX/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.PNG> <br />

- ### Ensemble Learners

- #### Balanced Random Forest Classifier <br />
Using the Balanced Random Forest Classifier we can see the balanced accuracy score was 79%, the precision for high risk was was only 4% and the sensitvity for high risk was only 67% but for low risk was up to 91%.
    <br /><br />
    <img src = https://github.com/AaronAKTX/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForest.PNG> <br />

- Easy Ensemble Classifier<br />
Using the Easy Ensemble AdaBoost Classifier we can see the balanced accuracy score was up to 93%, the precision for high risk was was only 7% and the sensitvity for high risk was up to 91% and for low risk was up to 94%.
    <br /><br />
    <img src = https://github.com/AaronAKTX/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble.PNG> <br />
    
## Summary
None of the models were great and I would not recommend any of them at this point to the banking institution. The precision in finding high risk never exceeded 7% in any of the models.  Also, in most of the models the sensitivity did not exceed 66%. This means that one third of high risk loans would pass the model without being detected. This is not good business for the bank. The Easy Ensemble Classifier was by far the best predictor, it had a sensitivity of 91% for high risk credit. While this would catch nearly all potentially high risk credits, only being 7% precise means it would also flag a high number of low risk loans as high risk. In my opinion, this low precision is not good enough to sign off on this model. More work must be done to hone the classifier to a point that brings the precision higher while keeping the high sensitivity.

    
    
