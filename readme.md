# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### L Dedeepya

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Initially model Error was much without tuning of any parametrs after feature engineering model performed well

### What was the top ranked model that performed?
TODO: WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: Exploratory Data Analysis (EDA) is the set of tools and processes that allows us to understand data better. This helps in identifying outliers, and visualizing feature distributions.EDA helped me to understand data much better that helped me building a good model.I have added new features like day,month,year,hour by splitting datatime field into day,month,year,hour and also changed the category of some columns like season,weather to categorical type.

### How much better did your model preform after adding additional features and why do you think that is?
TODO: As more the data to some extent the more the model performance will be so tt performed quite good with score 0.49957  

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: After tuning hyperparameters the RMSE error reduced to 0.49012

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: I would spend time trying different hyperparameters to increase model performance much better

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|"time_limit=600"|'presets="best_quality"'|'verbosity=2'|1.39679|
|add_features|"time_limit=600"|'presets="best_quality"'|'verbosity=2'|0.49705|
|hpo|'num_trials=7'|"search_strategy='auto'"|"'scheduler':'local'"|0.49519|

TODO: Replace the image below with your own.

![model_train_score.png](nd009t-c1-intro-to-ml-project-starter/model_train_score.png)
### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](nd009t-c1-intro-to-ml-project-starter/model_test_score.png)

## Summary
TODO: In this project i used AutoGluon library to train several models for the Bike Sharing Demand competition in Kaggle. I used Tabular Prediction to fit data from CSV files provided from the competition. Having loaded the train test data I have intially trained a model with some parameters which intially gave me high error. On doing Feature Engineering The performance of the model got improved, tuning model with different hyperparameters made my model perform well and reduced the error further.Having done this I would further work on making model performance better and upto the mark.
