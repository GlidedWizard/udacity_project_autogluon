# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Abdelrahman Moataz


## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?


I realized that the model needed either more data or more features

### What was the top ranked model that performed?
LightGBMLarge 

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I found the distribution of the data using a histogram and decided to add new features using the datetime column (hours and days)


### How much better did your model preform after adding additional features and why do you think that is?
As shown in the graph the RMSE substantially dropped after I used the 2 new features. Its definetly because the model had access 
to more data that way

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
it was a bit better but not much since autogluon is so powerfull 

### If you were given more time with this dataset, where do you think you would spend more time?
adding more features

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
| Model         | Hyperparameters Modified   | Kaggle Score |
|---------------|----------------------------|--------------|
| initial       | None                       | 1.79487      |
| add_features  | Added features             | 0.61834      |
| hpo           | Hyperparameter optimization| 0.52954      |



### Create a line plot showing the top model score for the three (or more) training runs during the project.



![model_test_score.png](model_test_score.png)



## Summary

In my project on predicting bike sharing demand with AutoGluon, I discovered that enhancing the model's performance required either more data or additional features. Through exploratory data analysis, I found insights into the data distribution using histograms and leveraged the datetime column to create new features, such as hours and days. The inclusion of these features notably improved the model's performance, as evidenced by the significant drop in RMSE. Although experimenting with different hyperparameters yielded only marginal improvements, the AutoGluon framework demonstrated its robustness even with default settings. Given more time, I would focus on further enriching the feature set to enhance model accuracy. Overall, the project underscored the iterative nature of model development and the efficacy of AutoGluon in simplifying the process while delivering competitive results.
