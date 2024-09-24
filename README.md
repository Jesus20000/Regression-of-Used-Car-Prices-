# Regression of Used Car Prices

## Overview
This project aims to predict the prices of used cars using various features such as mileage, model year, and engine specifications. It utilizes the CatBoost regression model, enhanced through hyperparameter optimization via Optuna.

## Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- re
- warnings
- optuna
- catboost
- scikit-learn

## Data
- `train.csv`: Contains the training data with features and prices of used cars.
- `test.csv`: Contains the testing data for which the prices are to be predicted.

## Analysis Steps
1. **Data Loading**: Load the training and test datasets.
2. **Data Cleaning**: Handle missing values, extract features, and convert categorical variables.
3. **Feature Engineering**: Create new features such as vehicle age, mileage per year, horsepower, and cylinder count.
4. **Data Visualization**: Analyze the distribution of car prices and relationships between features.
5. **Model Training**: Utilize CatBoost Regressor with K-Fold cross-validation.
6. **Hyperparameter Optimization**: Use Optuna to find the best model parameters.

## Insights
- The model effectively predicts car prices based on the features provided.
- Feature importance analysis can further improve the model by identifying key variables influencing price.

## Conclusion
The model demonstrates a promising performance in predicting used car prices, with the potential for further refinement through additional data and advanced techniques.
