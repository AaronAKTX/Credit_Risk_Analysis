# Credit_Risk_Analysis

# Main Objective

 The main objective of this challenge was to build different machine learning models that can help determine credit risk. Once complete, the models were evaluated to determine if any were suitable options to use or to use as a starting place to grow from.


## Machine Learning Models

- ### OVERSAMPLING
  
  - #### RandomOverSampler algorithm
Using the RandomOverSampler algorithm to resample the dataset before training the logistic regression classifier did not yield great results. Below we can see the balanced      accuracy score was 64%, the precision for high risk was was only 1% and the sensitvity for high risk  was only 62% and for low risk only 65%.
    <br />
    <img src = https://github.com/AaronAKTX/Amazon_Vine_Analysis/blob/main/resources/vine%20reviews.PNG> <br />

  - #### SMOTE algorithm  
Using the SMOTE algorithm to resample the dataset before training the logistic regression classifier did also not yield very promising results. Below we can see the balanced      accuracy score was 63%, the precision for high risk was was only 1% and the sensitvity for high risk  was only 62% and for low risk only 64%.
    <br />
    <img src = https://github.com/AaronAKTX/Amazon_Vine_Analysis/blob/main/resources/vine%20reviews.PNG> <br />

- ### UNDERSAMPLING

  - #### CluserCentroids resampling
Using the CluserCentroids algorithm to undersample the dataset before training the logistic regression classifier did not prove to be a valuable prediction tool. Below we can see the balanced accuracy score was 51%, the precision for high risk was was only 1% and the sensitvity for high risk  was only 59% and for low risk only 43%.
    <br />
    <img src = https://github.com/AaronAKTX/Amazon_Vine_Analysis/blob/main/resources/vine%20reviews.PNG> <br />

- ### COMBINATION SAMPLING
  
  - #### SMOTEENN model
Using the SMOTEENN algorithm to combine over and under sampling of the dataset before training the logistic regression classifier did not prove to be a valuable prediction tool. Below we can see the balanced accuracy score was 62%, the precision for high risk was was only 1% and the sensitvity for high risk was only 71% and for low risk only 54%. It is notable that of all the methods tried thus far, SMOTEENN yielded the highest sensitivity for High Risk credit accounts.
    <br />
    <img src = https://github.com/AaronAKTX/Amazon_Vine_Analysis/blob/main/resources/vine%20reviews.PNG> <br />

- BalancedRandomForestClassifier model

- EasyEnsembleClassifier model
