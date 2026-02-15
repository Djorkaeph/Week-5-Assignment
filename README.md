# Week-5-Assignment
I began my assignment by installing and importing pandas as pd and loading my churn dataset, setting CustomerID as the index column. Next, I installed PyCaret and imported the necessary tools to create, load, and use classification models. I then set up a new PyCaret classification experiment object and assigned it to the variable automl.

The next step was to identify the best model, which turned out to be the AdaBoost Classifier. I evaluated this model, generated plots, and examined its confusion matrix: 1,551 instances were correctly predicted as 0, and 561 instances were correctly predicted as 1. I then tested the model on the last row of the dataset and found that it predicted incorrectly for this customer — the customer ended up churning, even though the model predicted they would not.

Looking at predictions across the entire dataset, the model achieved approximately 73% accuracy. For the first five rows, the model correctly predicted churn for 3 out of 5 cases. However, when analyzing predictions for all rows, I noticed that the model made very few churn predictions, suggesting a potential issue with its performance.

Finally, I saved and loaded the best model and checked predictions again; the prediction score remained the same.

In conclusion, this model does not effectively predict churn. It tends to predict that most customers will not churn and rarely predicts when they actually do, indicating that it may not be suitable for identifying high-risk customers without further tuning or using a different modeling approach.
