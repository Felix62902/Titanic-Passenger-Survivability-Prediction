# Data Files:
train.csv: Contains the training data.
test.csv: Contains the testing data.
submission.csv: Contains the prediction results.

In this project, the titanic data set is split into two. 80% of the data is used for training, and 20% used for testing.
It utilises a heatmap to find series that are highly negatively correlated (e.g. Passenger class and Sex), and data that are highly correlated (Fare) to be selected as Features to be used to 
train the model. The model is trained using only the training data to provide an unbiased result, the RandomForestClassifier model is selected for the prediction. The model is then passed the
testing data which does not contain the "Survived" columnn as it is what the model is predicting. The result is then put into the submission.csv file which contains two columns ( PassengerId and
Survived). 1 means Survived while 0 means deceased.
The resulting model has an prediction accuracy of 75.1% (as revealed on submission on Kaggle)
