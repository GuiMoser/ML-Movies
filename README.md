# Machine Learning Movies

Training a regression model to predict movie scores.
In this notebook we see all the steps for training a regression model.

EDA - Analyzes the correlation of columns with a matrix and plots graphs for better analysis of columns.
Encoding - Performs encoding using MultiLabelBinarizer to transform the column with film genres into different columns that can be used as FEATURES.
Scaling - After separating the sets into Train Validation and Test, uses the MinMaxScaler.
Cross-Validation - Performs Cross-Validation on three different model types (LinearRegression, LightGBMRegressor, RandomForestRegressor) and analyzes the scores of each one.
Hyperparemeter Tuning - Defines a function using GridSearchCV to find the hyperparameters with the best R2 Score for LightGBM and RandomForest.
Final Model - Trains the final model with the best hyperparameters and makes predictions on the test set.

This notebook uses a Dataset containing information about movies which appears on IMDB website: 
https://www.kaggle.com/datasets/adriankiezun/imdb-dataset-2023

Data was preprocessed to include only movies which were released after 1970 and currently have over 50 000 ratings. Additionally there were selected only these movies whose budgets and gross' are denominated in USD to avoid discrepancies.

id - movie's ID used by IMDB repository
primaryTitle - title in English
originalTitle - original title in native language
isAdult - parental guidance
runtimeMinutes - total runtime in minutes
genres - genres
averageRating - final rating, based on all the ratings
numVotes - total number of votes (ratings)
budget - total budget in USD
gross - total gross worldwide in USD
release_date - release date, first occurrence
directors - directors
