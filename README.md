# Taxi Fare Prediction 🚖📊

## Summary

This project focuses on predicting taxi fares using a variety of machine learning techniques. The dataset used includes features such as pickup and dropoff locations, times, and passenger counts. The goal is to build and evaluate models that can accurately predict the fare amount based on these inputs.

## Project Steps

1. **Fetch the Data 📥**
    - Setup the initial Python environment.
    - Load necessary libraries: `numpy`, `pandas`, `matplotlib.pyplot`, and `sklearn`.
    - Read the dataset from a CSV file and explore the data types.

2. **Feature Engineering 🛠️**
    - Add new features: `abs_diff_longitude` and `abs_diff_latitude`, representing the "Manhattan vector" from the pickup location to the dropoff location.

3. **Data Cleaning 🧹**
    - Check for missing values and remove rows with any missing data using `pandas.DataFrame.dropna`.
    - Visualize some examples and remove outliers to ensure data quality.

4. **Model Training and Evaluation 🤖**
    - **Normal Equation:**
        - Prepare the input matrix and target variable.
        - Train a linear regression model using the normal equation method.
        - Evaluate the model on the test dataset.
    - **Gradient Descent:**
        - Utilize `sklearn.linear_model.LinearRegression` to train a model.
        - Predict and evaluate the model on the test dataset.
    - **Decision Tree:**
        - Use `sklearn.ensemble.RandomForestRegressor` for model training.
        - Perform hyperparameter tuning using `GridSearchCV`.
        - Train and evaluate the model using the best parameters.

5. **Feature Analysis and Visualization 📈**
    - Parse and extract date-related features from the `pickup_datetime` column.
    - Analyze the impact of different features (e.g., `Month`, `Year`, `Hour`, `passenger_count`) on the fare amount using visualizations with `seaborn` and `matplotlib`.

## Contributors ✍️

- Sana Shamma
- Salwa Shamma
- Samah Shamma
