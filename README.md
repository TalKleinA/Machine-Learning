# Machine-Learning
## Churn prediction project plan:
### EDA:

* look for duplicates, missing values, data types and weird values. 
* take care of outliers or anomalies. 
* Visualize some of the features in regards to the target in order to understand what affects customers to leave.
* Create a cohort analysis to understand the effect of joining time on loyalty.

### Preprocessing:

* change types and encoding. Add 2 more features of has_phone and has_internet. Unite all the tables to one dataset.
* It will be interesting to see how the total time a customer exists in the company behaves on regard to different features.
* Split the source data into a training set, a validation set, and a test set.
* Scale the data using minmax 
* Fix the imbalance using upsampling/downsampling and class_weight='balanced'. We will save it to a new dataset and compare the results in both cases.
* Create a new feature `ClientsCluster` using unsupervised model Kmeans without using the target in order to improve the final model's predictions. Try to predict with and without this and compare the results.

### Baseline:

* Use Decision Tree or Logistic regression as a baseline model to perform a sanity test to the models up ahead.

### Training:

* Fit the model on the training set using different models:
    - Random forest
    - XGboost
    - Deep learning - Neural network (not sure which yet)
* Fine tuning using gridsearchCV and the validation set

### Testing:

* Test the data on the test set and evaluate it using AUC-ROC since it's a classification problem. We will also check the Accuracy metric and F1 score to have a fuller understanding of the models.



