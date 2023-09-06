# Module 12 Report Template

## Overview of the Analysis
This notebook builds a model that can identify the creditworthiness of borrowers, solving a classification problem of imbalanced data. We use the data provided under Resources which contains historical lending activity from a peer-to-peer lending services company.

A logistic regression model is used on both the original dataset and the resampled data(RandomOverSampler module from the imbalanced-learn library was used for resampling)

For both cases we followed this steps (data was split for training and testing):
1) Counted the values of the target classes.
3) Trained a logistic regression classifier by instantiating the model, fitting the model with training data and predicting y values using testing data. 
4) Calculated the balanced accuracy score.
5) Generated a confusion matrix.
6) Generate a classification report.

## Results

* Machine Learning Model 1:
  - #### Accuracy score:
    0.952
  - #### Precision score:
    Healthy loan: 1.00 <br> 
    High Risk loan: 0.85
  - #### Recall scores:
    Healthy loan: .99 <br> 
    High Risk loan: .91
  - #### f1 score:
    Healthy loan: 1.00 <br> 
    High Risk loan: .88

* Machine Learning Model 2:
  - #### Accuracy score:
    0.993
  - #### Precision score:
    Healthy loan: 1.00 <br> 
    High Risk loan: 0.84
  - #### Recall scores:
    Healthy loan: .99 <br> 
    High Risk loan: .99
  - #### f1 score:
    Healthy loan: 1.00 <br> 
    High Risk loan: .91

## Summary

When looking at the two different machine learning models, we can see that for this analysis resampling the data works best as it yields a better accuracy, f1 and recall scores. It is important that the model minimizes the false negatives as not detecting a high risk loan could negatively impact the company's performance. 

It is important to note that the excercise did not require us to scale the data, I would recommend this to improve the model.
