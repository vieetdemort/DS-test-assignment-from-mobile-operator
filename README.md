# DS-test-assignment-from-mobile-operator

```python
print("Hi, my name is Nazim! ")
```
Binary classification problem:
"1" - the subscriber is a driver (belongs to the drivers segment),
"0" - the subscriber is not a driver (does not belong to the drivers segment).

The files tabular_data.csv and hashed_feature.csv ̶ here are descriptive characteristics for 4084 subscribers ("ID" is the subscriber ID).
The train.csv file ̶ is the target label data (the subscriber's belonging to the driver segment).
File test.csv ̶ is the list of subscribers for which we want to make a prediction, by which we will evaluate the quality of the model. The ROC-AUC is used as the metric.

"The file tabular_data.csv contains the numeric data on the activity of subscribers for 12 periods.
- period - period number (periods are consecutive, 1 is the newest)
- id - subscriber ID
- feature_0 - feature_49 - data on the subscriber's activity in the corresponding period.


"File hashed_feature.csv - here is the set of hashed values of one categorical variable for the subscriber.
- id - subscriber's identifier
- feature_50 - hash of the value of the categorical variable.


"File train.csv - here is the data with the target label.
- id - identifier of the target
- target - target label value (1 - belongs to drivers segment, 0 - does not belong to drivers segment).


"test.csv file - list of subscribers for which you want to make predictions with your models.
- id - the subscriber's identifier
- score - the probability that the caller belongs to the drivers segment (class "1"). This probability is determined by your model.


You need to build your model on the subscribers whose target label is contained in the train.csv file. 
To do this, you need to use data from tabular_data.csv and hashed_feature.csv files. 
Then, using your model, you need to fill in the score column for the subscribers from the test.csv file - the probability that the subscriber belongs to the driver segment. 
Note that you need to predict the fact of the relation to the drivers segment, without reference to the period.

P.S. The target in ROC-AUC is 90%+

```python
print("Thank You")
```
