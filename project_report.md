# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Jiya Chawla

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
My train data had more columns than the test data. So, two columns had to be removed from the train data.

### What was the top ranked model that performed?
WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
the results of the eda were interesting, we fond various insights like patterns in bike demand related to time of the day, season etc. I added new features by using insights like hour of the week, day etc.

### How much better did your model preform after adding additional features and why do you think that is?
There was an improvement of 71.322% after the adding of new features compared to the initial model. Model performed quite better after the addition of new features. It is because the new features allow the model to identify new patterns and relationships in data.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
There was an improvement of 70.74% compared to the initial model. While it was better than the initial performance, there's a slight decrease compared to the second model.

### If you were given more time with this dataset, where do you think you would spend more time?
I would work more on eda and feature engineering to further explore the dataset and improve the model's performance.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|None|None|None|1.80223|
|add_features|None|None|None|0.51683|
|hpo|RF|CAT&XGB|GBM&FASTAI|0.52717|

### Create a line plot showing the top model score for the three (or more) training runs during the project.


[model_train_score(1).png](img/model_train_score(1).png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.


[model_test_score(1).png](img/model_test_score(1).png)

## Summary
The project helped me understand how AutoGluon assists in the machine learning process by the example of predicting bike sharing demand. By combining techniques like eda, feature engineering, and hyperparameter tuning, we were able to achieve great improvement in model performance. 
