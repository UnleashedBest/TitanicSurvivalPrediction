# Titanic Survival Prediction Dataset

## Overview

This dataset contains information about the passengers on the Titanic, including whether they survived or not. The goal is to use this information to predict whether a passenger would have survived or not based on their characteristics.

## Data Source

The dataset was obtained from Kaggle, and it consists of two CSV files: `train.csv` and `test.csv`. The `train.csv` file contains the data used for training and validating machine learning models, while the `test.csv` file contains the data used for testing the final model.

## Data Description

The following is a description of each feature in the dataset:

- `PassengerId`: The ID number of each passenger
- `Survived`: Whether the passenger survived (0 = No, 1 = Yes)
- `Pclass`: The passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: The name of the passenger
- `Sex`: The gender of the passenger (male or female)
- `Age`: The age of the passenger
- `SibSp`: The number of siblings or spouses the passenger had on board
- `Parch`: The number of parents or children the passenger had on board
- `Ticket`: The ticket number of the passenger
- `Fare`: The fare paid by the passenger
- `Cabin`: The cabin number of the passenger
- `Embarked`: The port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Data Preparation

The following data preparation steps were applied to the dataset:

- Missing values were imputed using the median value for numerical features and the mode value for categorical features.
- The `Name` feature was used to extract the title of each passenger, which was then used to create a new feature called `Title`.
- The `Ticket` feature was dropped from the dataset as it did not provide any useful information for predicting survival.
- The `Cabin` feature was dropped from the dataset due to a large number of missing values.
- The `Embarked` feature was imputed using the mode value.

## Exploratory Data Analysis

The following insights were obtained from the dataset:

- The majority of the passengers were in third class.
- The survival rate for females was much higher than for males.
- Passengers who were younger had a higher chance of survival.
- Passengers with fewer siblings or spouses on board had a higher chance of survival.
- Passengers who paid a higher fare had a higher chance of survival.

## Model Building

The following machine learning models were trained on the dataset:

- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Random Forest
- Gradient Boosting

The models were evaluated using cross-validation, and the best performing model was selected for further tuning.

## Model Tuning

The selected model was further tuned using grid search to find the optimal hyperparameters.

## Conclusion

Based on the analysis of the dataset, it can be concluded that gender, age, and passenger class were important factors for predicting survival on the Titanic. The best performing machine learning model was able to achieve an accuracy of 83% on the test dataset, which is a reasonable performance given the complexity of the problem.
