On this project, we will fit our model using the same steps as before (IntrotoSimpleLinearRegression, LeastSquaresRegressionExample, e.t.c), except this time we will expose it only to the training data
We have handed four parameters to the splitting function:
	X: Contains the features on whivh we will be training the model. In this case: exports
	y: The response variable which we are training to predict. In this case: Exchange rate
	test_size: Value between 0 and 1: The proportion of our dataset that we wabt to be used as test data. Typically 0.2
	Random_state: Ensures the random nature in which rows are picked to be in the test set is the same each time the split is carried out
As we fit the model to the training data, we provide it with the training features and their responses. This it can Learn which data points map to which output, as is required of the model training process

Observation:
Mean squared error is higher on the test set than the train set, indicating poor predictive accuracy
R-squared is lower on the test set, including a worse fit on the test set
These results indicate a concept in machine learning model fitting known as overfitting.

Conclusion:
In this train we have been introduced to:
	The concept of unseen data, from the perspective of the model
	Splitting a dataset into training and testing subsets
	Calculating or interpreting model parameters(slope, intercept) using the training set
	Assessing the accuracy and fit of the model on the set 
