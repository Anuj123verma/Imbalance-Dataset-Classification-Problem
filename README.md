# Imbalance-Dataset-Classification-Problem
In this I will describe how to handle the imbalance datasets for classifications.
Generally we get a very high accuracy in case of imbalance datasets and we think model is working fine but it is not actually the case. If we test this model on the test datasets it will give the very less accuracy, the reason for this is that it is not considering the datapoints which are very low and our test dataset wants to detect the points which are low in training datasets. For example, credit card fradulent detection.
So, in case of imbalance dataset we do not consider accuracy but we consider the ROC curve.
Before applying any model to the imbalance dataset we have to balance it,either do undersampling or oversampling,but remember in case of oversampling don't use synthetic points means don't use techniques like smote, you can use RandomUnderSampler or RandomOverSampler to do this task, but always take care of the ratio, beacuse that lead to overfiiting also and your model behave not that good as expected.
You can also remove some columns that have high correlation, so always try to analyze the data well before dooing any ching preprocessing.
Models like xgboost regressor, random forest regresssor, etc. are quite useful for these type datasets.
I am attaching the code and report.
