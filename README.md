# Supervised_Machine_Learning</br>
# The Credit Risk Analysis</br>
## Overview of the analysis</br>
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.</br>
We are now ready to apply machine learning to solve a real-world challenge </br>
Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes. </br>
We are going to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.</br>
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we will oversample the data using </br>
* The RandomOverSampler and SMOTE algorithms, </br>
* Undersample the data using the ClusterCentroids algorithm. </br>
  Then, we use a combinatorial approach of </br>
* Over- and undersampling using the SMOTEENN algorithm. </br>
  Next, we compare two new machine learning models that reduce bias,</br>
* BalancedRandomForestClassifier </br>
* EasyEnsembleClassifier to predict credit risk.</br>
  We will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.</br>
## Results </br>
 We the raw data needs cleaning and we are converting it into a dataframe,by defining X as a multidimensional array and y as the target .</br>
 We are going to generate the following :</br> 
 * Calculate the accuracy score of the model.
 * Generate a confusion matrix.
 * Print out the imbalanced classification report.
   We are going to compare the values of "high risk" on "accuracy score" and "imbalanced classification report" on each case .</br>
 INSERT IMAGES OF DF,X,Y 
 ![Multidimentional array X]()
 ![Target y]()
## Resampling Models to Predict Credit Risk </br>
### The RandomOverSampler </br>
In random oversampling, instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced.</br>
![Accuracy score]()</br>
![]()</br>
From the above results we know

### SMOTE algorithms</br>
![]()</br>
![]()</br>
From the above results we </br>

### Undersample using ClusterCentroids algorithm </br>
![]()</br>
![]()</br>
From the above results we </br>

### Over and undersampling using the SMOTEENN algorithm </br>
![]()</br>
![]()</br>
From the above results we </br>

### BalancedRandomForestClassifier</br>
![]()</br>
![]()</br>
From the above results we </br>

### EasyEnsembleClassifier</br>
![]()</br>
![]()</br>
From the above results we </br>
