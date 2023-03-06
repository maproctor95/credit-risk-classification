# Credit Risk Report

## Overview of the Analysis
* Using a machine learning model, I will try to determine which loans are healthy (low-risk) or non-healthy (high-risk) based on the loan status provided by the lending company. 

* Using the dataset provided by the lending company, I created a Logistic Regression Model that generated an accuracy score of 95%. Although the model generated a high-accuracy, the models recall value (0.91) for non-healthy loans is lower than the recall value (0.99) for healthy loans. This indicates that the model will predict loan status's as healthy better than being able to predict loan status's as non-healthy. This is due to the dataset being imbalanced, meaning that most of the data belongs to one class label (in this case healthy loans greatly outweighed non-healthy loans).

* Using the dataset provided by the lending company, I created a Logistic Regression Model fit with the oversampled data that generated an accuracy score of 99%, which turns out to be higher than the model fitted with imbalanced data. The oversampled model performs better due to the dataset being balanced. The models non-healthy loans recall value increased from 0.91 to 0.99 indicating that the model does an exceptional job in catching mistakes such as labeling non-healthy (high-risk) loans as healthy (low-risk).

## **Results**

###Logistic Regression Model fitted with Imbalanced Data: 

* The model fitted with imbalanced data has a higher possibility of making these mistakes: 

  * a healthy loan (low-risk) is classified as a non-healthy loan (high-risk).
  * a non-healthy loan (high-risk) is classified as a healthy loan (low-risk).


### Logistic Regression Model fitted with Balanced (oversampled) Data:

* The model fitted with balanced (oversampled) data has a much lower possibility of making these mistakes: 

  * a healthy loan (low-risk) is classified as a non-healthy loan (high-risk).
  * a non-healthy loan (high-risk) is classified as a healthy loan (low-risk).


## **Summary**
* Model fitted with Imbalanced Data: 
  
  * 56 (FALSE POSITIVES) --> The actual value is healthy and the predicted value is non-healthy 


  * 102 (FALSE NEGATIVES) --> The actual value is non-healthy and the predicted value is healthy


* Model fitted with Balanced Data: 
  
  * 4 (FALSE POSITIVES) --> The actual value is healthy and the predicted value is non-healthy 


  * 116 (FALSE NEGATIVES) --> The actual value is non-healthy and the predicted value is healthy
