# Supervised_Machine_Learning</br>
# The Credit Risk Analysis</br>
## Overview of the analysis</br>
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.</br>
We need to employ different techniques to train and evaluate models with unbalanced classes. </br>
We are going to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.</br>
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we will  </br>
* Oversample the data using the RandomOverSampler and SMOTE algorithms, </br>
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
   We are going to compare the values of "high risk" on "accuracy score" and "imbalanced classification report" on each case and F1 score.</br> 
   F1 Score is the weighted average of Precision and Recall. Therefore, this score takes both false positives and false negatives into account. </br> 
   Intuitively it is not as easy to understand as accuracy, but F1 is usually more useful than accuracy, especially if you have an uneven class distribution.</br>
   
 ![Multidimentional array X](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/muliDX.png)
 ![Target y](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/y-target.png)
## Resampling Models to Predict Credit Risk </br>
### The RandomOverSampler </br>
In random oversampling, instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced.</br>
![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/randomsampling.png)</br>
From the above results we know accuracy  as 0.6576123702173772 i.e. 65% and F1 scre for high risk is 0.02

### SMOTE algorithms</br>
![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/SMOTE.png)</br>
From the above results we know the accuracy as 0.6600566482045773 and the F1 score is again 0.02</br>

### Undersample using ClusterCentroids algorithm </br>
![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/undersampling.png)</br>

From the above results we know accuracy is 0.5453770295177319 and F1 as 0.01 </br>

### Over and undersampling using the SMOTEENN algorithm </br>
![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/SMOTEENN_Accu.png)</br>

![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/SMOTEENN_%20ICR.png)</br>
From the above results we get the accuracy as 0.5453770295177319,F1 score 0.02 </br>

### BalancedRandomForestClassifier</br>
![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/BRC.png)</br>

From the above results we get the accuracy as 0.775955077383323, F1 score for high risk as 0.07 </br>

### EasyEnsembleClassifier</br>
![](https://github.com/ramyasnl/Supervised_Machine_Learning/blob/master/SSMOD17/EEAdaC.png)</br>
![]()</br>
From the above results we know the accuracy is 0.9322840931193213 that is 93% and the average F1  is 96% which is BEST among all other algorithms.</br>
## Conclusion 
 Among all the algorithms The EasyensembleClassifier can be the best option because of the accuracy on the other hand the F1 scores are not too good ,</br>
 Using only the above algoritms may not be a good decision to choose the deserving candidates or to eliminate the high risk candidates. 
 
