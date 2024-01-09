# Machine Learning Pipelines Exploration

This Python script explores the concept of machine learning pipelines using the scikit-learn library. The script focuses on constructing a pipeline for preprocessing and training a regression model on the Abalone dataset.

## Prerequisites

Make sure you have the required libraries installed. You can install them using:

`pip install numpy pandas scikit-learn`

The script performs the following steps:

    Data Loading:
        Loads the Abalone dataset from the UCI Machine Learning Repository.

    Data Preprocessing:
        Creates missing values in the dataset to simulate a real-world scenario.
        Splits the dataset into training and testing sets.

    Pipeline Construction:
        Constructs a machine learning pipeline using scikit-learn's Pipeline class.
        Uses a ColumnTransformer to handle both numerical and categorical features separately.
        Applies imputation and scaling to numerical features.
        Applies imputation and one-hot encoding to categorical features.

    Model Training:
        Uses a Linear Regression model as the default regression model in the pipeline.
        Defines a search space with different regression models (Linear Regression, Ridge, and Lasso) and their hyperparameters.

    Grid Search:
        Performs grid search using GridSearchCV to find the best pipeline and hyperparameters.

    Results:
        Prints the best regression model and its hyperparameters.
        Prints the hyperparameters of the categorical preprocessing step.
