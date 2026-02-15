# Week-5-Assignment
I will be going over my process while working this assignment and my finding. 
After installing and importing pandas as pd, I imported my churn data as set customerID as the index column.
I then installed Pycaret and imported the necessary Pycaret tools needed to create. load and use classification models
I set up a new pycaret classification experiment object and assigned it to the variable automl
The next step was to look for the best model which turned out to be the Ada Boost Classifier
I then evaluated,plotted and looked at a confusion matrix for my best model
1551 classes were correctly predicted as 0 and 561 classes we correctly predicted as 1 on the confusion matrix.
Next I predicted the class of the last row of the data using the best model and I found that the model predicted incorrectly for this customer. This customer ended up churning even though the model predicted they would not.
I then looked at predictions for the whole dataset and the model appears to be 73% accurate.
The model went 3/5 when predicting churn for the first five columns.
When analyzing the predictions for all the rows in my dataset I noticed very few churn predictions from my model which may indicate an issue with the model.
The last few steps were to save and load our best model and to check the new predictions using the model.
The prediction score remained the same.
In conclusion, It appears that this model does not correctly predict churn as the model predicts that most customers will not churn and very rarely predicts when they do.
