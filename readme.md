# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### L Dedeepya

## Initial Training
Initially model Error was much without tuning of any parametrs after feature engineering model performed well


## Exploratory data analysis and feature creation

TODO: Exploratory Data Analysis (EDA) is the set of tools and processes that allows us to understand data better. This helps in identifying outliers, and visualizing feature distributions.EDA helped me to understand data much better that helped me building a good model.I have added new features like day,month,year,hour by splitting datatime field into day,month,year,hour and also changed the category of some columns like season,weather to categorical type.
As more the data to some extent the more the model performance will be so tt performed quite good with score 0.49957  

## Hyper parameter tuning

After tuning hyperparameters the RMSE error reduced to 0.49012



![model_train_score.png](nd009t-c1-intro-to-ml-project-starter/model_train_score.png)
### line plot 


![model_test_score.png](nd009t-c1-intro-to-ml-project-starter/model_test_score.png)

## Summary
In this project i used AutoGluon library to train several models for the Bike Sharing Demand competition in Kaggle. I used Tabular Prediction to fit data from CSV files provided from the competition. Having loaded the train test data I have intially trained a model with some parameters which intially gave me high error. On doing Feature Engineering The performance of the model got improved, tuning model with different hyperparameters made my model perform well and reduced the error further.Having done this I would further work on making model performance better and upto the mark.
