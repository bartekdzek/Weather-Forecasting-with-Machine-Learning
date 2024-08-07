# Weather-Forecasting-with-Machine-Learning

## Weather Machine Learning Project

## Overview

This project involves analyzing and predicting weather data using machine learning techniques. The dataset contains daily weather observations in Fahrenheit from the New Orleans Airport station. The goal is to build a predictive model to estimate the maximum temperature for the following day based on historical data.

## Data Description

The dataset, `local_weather.csv`, contains daily weather records with the following columns:
- **PRCP**: Precipitation (in tenths of mm)
- **SNOW**: Snowfall (in tenths of mm)
- **SNWD**: Snow depth (in mm)
- **TMAX**: Maximum temperature (in tenths of degrees Fahrenheit)
- **TMIN**: Minimum temperature (in tenths of degrees Fahrenheit)

### Station Details
- **Name**: New Orleans Airport, LA US
- **Network ID**: GHCND:USW00012916
- **Latitude/Longitude**: 29.99755°, -90.27772°
- **Elevation**: -1 m

## Project Steps

1. **Data Loading and Preparation**
   - Load the dataset using pandas.
   - Inspect and clean the data by handling missing values.
   - Convert data types and address any anomalies.

2. **Exploratory Data Analysis (EDA)**
   - Plot temperature trends and precipitation data.
   - Aggregate and visualize annual and monthly precipitation totals.
   - Analyze correlations between features and the target variable.

3. **Feature Engineering**
   - Create rolling mean features for temperature.
   - Compute new features such as temperature range and logarithm of precipitation.
   - Evaluate the impact of these features on model performance.

4. **Model Training and Evaluation**
   - Train a Ridge regression model to predict the maximum temperature for the next day.
   - Evaluate the model's performance using Mean Absolute Error (MAE).
   - Compare Ridge regression with Random Forest Regressor.

5. **Prediction and Results**
   - Use the best-performing model to predict the maximum temperature for the next day.
   - Analyze predictions and errors to enhance forecasting accuracy.

## Key Features Added

- **Rolling Means**: To capture trends in temperature over a 30-day window.
- **Temperature Range**: Difference between maximum and minimum temperatures.
- **Log Transformation**: Applied to precipitation to handle skewed distributions.

## How to Use

1. **Setup**: Ensure you have the required libraries installed:
   - `pandas`
   - `numpy`
   - `sklearn`

2. **Running the Notebook**: 
   - Load and clean the data.
   - Train and evaluate models.
   - Make future temperature predictions.

3. **Prediction for Tomorrow**: Use the function `predict_tomorrow` to forecast the maximum temperature for the next day based on the latest data.

## Results

The project demonstrates various methods for predicting weather data, including:
- Feature selection and engineering to improve model performance.
- Comparison of different machine learning models to identify the most effective approach.

## Acknowledgments

This project utilizes data from the New Orleans Airport weather station. Thanks to the Global Historical Climatology Network (GHCN) for providing the weather data.
