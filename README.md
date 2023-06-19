# Predicting-Temperature-in-London
Personal Project

The dataset used in this project is sourced from DataCamp.

### Task: 
Find the best model to predict temperatures in London!

### Background:
As the climate changes, predicting the weather becomes ever more important for businesses. Since the weather depends on a lot of different factors, you will want to run a lot of experiments to determine what the best approach is to predict the weather. In this project, you will run experiments for different regression models predicting the mean temperature, using `sklearn`.

You will be working with data stored in `london_weather.csv`, which contains the following columns:
- **date** - recorded date of measurement - (**int**)
- **cloud_cover** - cloud cover measurement in oktas - (**float**)
- **sunshine** - sunshine measurement in hours (hrs) - (**float**)
- **global_radiation** - irradiance measurement in Watt per square meter (W/m2) - (**float**)
- **max_temp** - maximum temperature recorded in degrees Celsius (°C) - (**float**)
- **mean_temp** - mean temperature in degrees Celsius (°C) - (**float**)
- **min_temp** - minimum temperature recorded in degrees Celsius (°C) - (**float**)
- **precipitation** - precipitation measurement in millimeters (mm) - (**float**)
- **pressure** - pressure measurement in Pascals (Pa) - (**float**)
- **snow_depth** - snow depth measurement in centimeters (cm) - (**float**)

## Instructions

Test three different regression models on historical London weather data.

For this project, you will use the London weather dataset from 1979 to 2021. The goal is to automatically process and test different models using sklearn. You will use weather data to predict the mean temperature on a given day.

The result of this project should be three different regression models (linear regression, decision tree regressor, and random forest regressor) and their results.

Perform exploratory data analysis, preprocessing, training, prediction, and evaluation of machine learning models to predict "mean_temp" from the london_weather.csv.

## My approach

Exploratory data analysis

1. Load the data from london_weather.csv to understand its contents

2. Determine the column names, data types, number of non-null vales

3. Convert 'date' column to datetime type

Data visualization

1. Explore the data by visualizing the features, and how the target variable, mean_temp, varies with each.

2. Based on the visualizations made in step 2, we find that we can pick a subset of features to predict the mean temperature.

Preprocess data

1. Use the imputer to account for missing values, and then normalize the features using the scaler. Make sure to split the data into train and test samples. 

Feature selection

1. PCA is used to reduce the dimensionality of the feature set, so that the reduced feature set explains 80% of the total variance. Scree plot is used to choose the number of components

Machine learning training and evaluation

1. Fit three regression models, linear regression, decision tree, and random forest regressor.

2. Training and evaluation the machine learning models using rmse.
