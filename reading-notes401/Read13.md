# How to Run Linear Regression in Python



## Boston Housing Data Set
The first step is to import the required Python libraries into Ipython Notebook.

This data set is available in sklearn Python module, so I will access it using scikitlearn. I am going to import Boston data set into Ipython notebook and store it in a variable called boston.


## Scikit Learn
is useful and robust library for machine learning in Python. It provides a selection of efficient tools for machine learning and statistical modeling including classification, regression, clustering and dimensionality reduction via a consistence interface in Python.

## Fitting a Linear Model

A **linear model** describes the relationship between a continuous response variable and the explanatory variables using a linear function. Simple regression models describe the relationship between a single predictor variable and a response variable.

## Predicting 
model. predict() : given a trained model, predict the label of a new set of data. This method accepts one argument, the new data X_new (e.g. model. predict(X_new) ), and returns the learned label for each object in the array.

## Training and validation data sets

In practice you wont implement linear regression on the entire data set, you will have to split the data sets into training and test data sets. So that you train your model on training data and see how well it performed on test data.

### How to do train-test split:
The simplest way to split the modelling dataset into training and testing sets is to assign 2/3 data points to the former and the remaining one-third to the latter. Therefore, we train the model using the training set and then apply the model to the test set. In this way, we can evaluate the performance of our model.


