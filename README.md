# Machine Learning Movies

## Project Description
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

## Dataset
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

## Objectives
- Perform exploratory data analysis.
- Encode categorical variables.
- Scale the data.
- Perform cross-validation on three different models.
- Perform hyperparameter tuning for LightGBM and RandomForest models.
- Train the final model with the best hyperparameters and make predictions on the test set.

## Tools and Libs used
- Python: Main language used for analysis.
- Pandas: Library for data manipulation and analysis.
- NumPy: Library for numerical operations.
- Matplotlib and Seaborn: Libraries for data visualization.
- Scikit-learn: Library for machine learning.
## Methodology
#### EDA
- Import libraries.
- Load the dataframes.
- Perform exploratory data analysis using summary statistics and data visualization.
#### Preprocessing
- Identify and treat missing values.
- Identify and treat outliers.
- Scale the data.
#### Encoding
- Use MultiLabelBinarizer to transform the column with film genres into different columns that can be used in the model.
#### Model Training and Evaluation
- Train and evaluate the models with different hyperparameters.
- Compare the performance of the models and select the best one.

## Learnings
- Data analysis: Interpreting and extracting valuable insights from large volumes of data.
- Data cleaning: Identifying and correcting missing, duplicate, and anomalous values.
- Creating graphics: Using matplotlib and seaborn to visualize data in an intuitive and informative way.
- Data preprocessing: Preparing Data for analysis, including cleaning and treat the data.
- Use of libraries and tools: Practical application of various libraries and tools from the Python ecosystem, such as Pandas, Numpy, Sklearn, Matplotlib and Seaborn.
- Data visualization: Creating very detailed graphs and other types of visualizations to identify patterns and trends.
- Data-driven decision making: Using insights derived from data analysis to guide strategic decisions.
- Regression Models: Train and evaluate regression models.
- Encoding: Transform multi-label data into a binary matrix for multi-label classification.
- Scaling: Scaling the data to have zero mean and unit variance.
- Hyperparameter Tuning: Perform hyperparameter tuning for regression models.
