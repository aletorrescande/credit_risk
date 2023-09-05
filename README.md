# credit_risk

This notebook builds a model that can identify the creditworthiness of borrowers, solving a classification problem of imbalanced data. We use the data provided under Resources which contains historical lending activity from a peer-to-peer lending services company.

A logistic regression model is used on both the original dataset and the resampled data (RandomOverSampler module from the imbalanced-learn library was used for resampling)

For both cases, we count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

The libraries and dependencies used are:
- numpy 
- pandas
- Path from pathlib 
- balanced_accuracy_score, confusion_matrix and classification_report_imbalanced from sklearn.metrics import 
