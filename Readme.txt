1. First of all, import the data and required libraries.
2. Then making the data validation, for avoiding the issues arising by mixed data types, as categorical data into strings.
3. preprocessor building.
Pipeline step for the preprocessing that handle the all data.
Preprocessor pipeline for all categorical data
For avoiding the data type errors, first of all convert all categorical columns to string.
Fill the missing column values.
Use one-hot encode to all categorical values. There might be a possibility of handling the unknown values that are present in the testing data, which may not be encounter in the training set. For that using encounter will help to ignore these problems.
Preprocessing pipeline for numerical value
Using the median value from the column to imputes the missing values in the numerical columns
For the each variable having mean zero and standard deviation one to scale

4.Pipeline for Preprocessing
Following steps are used for the pre-processing behaviors.
	1. Apply categorical pipeline.
	2. Apply numerical pipeline.
	3. drop the specified columns

5.building the model pipeline.
firstly apply the preprocessing steps to the raw data. And then using the eXtreme Gradient Boosted forest model to fit the pre processed data

6.Building Parameter Grid
Define a grid of hyper-parameters for the pipeline which will be tested in the grid search.
Initialize the grid search

7.Fit the grid search to identify the best model to training dataset.
And generate submission file accordingly

The model accuracy is 82.3%
