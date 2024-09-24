# Regression of Used Car Prices

## Overview
This project aims to predict used car prices based on various car features such as mileage, model year, engine specifications, transmission type, and more. The machine learning model used is CatBoost, a gradient boosting algorithm, which has been optimized using Optuna for hyperparameter tuning. The project involves data preprocessing, model building, and performance evaluation using mean squared error (MSE) as the evaluation metric.

## Libraries Used
- `pandas`: For data manipulation and preprocessing.
- `numpy`: For numerical computations.
- `matplotlib` & `seaborn`: For data visualization and feature analysis.
- `re`: For handling regular expressions to clean and extract features.
- `warnings`: To manage and suppress warnings during the workflow.
- `optuna`: For hyperparameter tuning and optimization of the model.
- `catboost`: A high-performance machine learning algorithm specialized for categorical features.
- `sklearn`: For data splitting and model evaluation using mean squared error (MSE) and other metrics.

## Data
The dataset includes features related to used cars, such as:
- `Model`: The brand and model of the car.
- `Mileage`: The total mileage of the car.
- `Year`: The year the car was manufactured.
- `Engine`: Engine capacity of the car.
- `Transmission`: The type of transmission (manual, automatic).
- `Price`: The price of the car (target variable).

The dataset was cleaned and preprocessed to remove missing values, standardize text columns, and create new features where applicable.

## Analysis Steps
1. **Data Preprocessing**:
    - Handled missing values and standardized the format of categorical columns (e.g., car models and transmission types).
    - Extracted useful numerical data from text columns like `Engine`.
    - Performed exploratory data analysis (EDA) to understand the distribution of features and their relationships with the target variable.

2. **Feature Engineering**:
    - Created new features such as the age of the car (`Current Year - Model Year`).
    - Converted categorical features to numerical using CatBoost's in-built handling of categorical data.

3. **Model Training**:
    - The CatBoost model was selected for its high performance on categorical data.
    - Hyperparameter tuning was performed using `Optuna` to find the optimal values for learning rate, depth, and other important parameters.

4. **Model Evaluation**:
    - The model was evaluated using `Mean Squared Error (MSE)` as the performance metric.
    - Cross-validation was used to validate the model’s performance on unseen data.

## Insights
- Car age and mileage were strong predictors of price.
- Transmission type also had a significant impact on price, with automatic cars generally priced higher.
- Other features such as engine capacity and model brand contributed to price variations.

## Conclusion
This project demonstrates the effectiveness of using CatBoost for regression tasks involving structured data with categorical features. Hyperparameter tuning with Optuna helped in optimizing the model to improve its accuracy.

## Requirements
- Python 3.8+
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - optuna
  - catboost
  - scikit-learn

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/Jesus20000/used-car-price-regression.git
