# Analytics_Vidhya_Job_A_Thon

This repository contains the solution file and dataset for analytics vidhya JOB-A-THON. Here you will find the notebook which has the method I used during the event to get the best solution possible.<br>

## Problem Statement:<br>
In this contest the dataset has 9 years of data for a country named Green Energy for green energy consumption in the country per hour. The problem statement was that using this data for training purposes we have to build a Machine Learning model which could predict for 3 years consumption of green energy in the future for every hour.

## Dataset:<br>
The dataset contains following columns:<br>
1. datetime<br>
2. energy<br>

The dataset has no null values.

## EDA and Feature Engineering:<br>
1. Upon plotting the values it is seen that the energy consumption shows a positive growth for increasing years in a linear manner.<br>
2. The dataset also has some outliers so they are removed.<br>
3. For prediction I needed more features which could fit the 3 years prediction horizon. So I added more features in our dataset according to seasonality.<br>
4. For that I made 8 different columns with a lag of 1 year each in every column based on energy.<br>
5. Using the datetime column I extracted different values like 'year', 'day', 'dayofweek', 'month', 'weekofyear' etc. and added these features to the dataset.<br>
6. The I used timeseriessplit from sklearn to split the time series data as it is sequential data so the data needs to be progressive while selecting training and test set and not random.<br>

## Modelling:<br>

For modelling purpoes I used two different algorithms:<br>
1. RandomForest<br>
2. XGBoost<br>
The best result was achieved using XGBoost.

## Tools used:<br>
<img src="https://github.com/zmwaris1/logos/blob/main/png-clipart-scikit-learn-python-scikit-logo-brand-learning-text-computer.png" alt="sickit-learn" height="40" style="vertical-align:top; margin:4px"><img src="https://github.com/zmwaris1/logos/blob/main/tutorial_matplotlib.png" alt="matplotlib" height="40" style="vertical-align:top; margin:4px"><img src="https://github.com/zmwaris1/logos/blob/main/Pandas_logo.svg.png" alt="Pandas" height="40" style="vertical-align:top; margin:4px">
<img src="https://github.com/zmwaris1/logos/blob/main/105040771-43887300-5a88-11eb-9f01-bee100b9ef22.png" alt="Numpy" height="40" style="vertical-align:top; margin:4px"><img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" alt="Python" height="40" style="vertical-align:top; margin:4px">

## Conclusion:<br>
Time series data is complex and if needed to be used for prediction one should make sure that sufficient data is present. The horizon for which the prediction is needed to be done must be based on the data available. Time series data is not easy to work with but at the same time it also give too much insight about the trend and pattern based on real world. For time series prediction XGBoost is one of the best algorithm to work with and gives most accurate predictions.

# Rank Secured

Secured 18th rank on the leaderboard.

<img src="https://github.com/zmwaris1/Analytics_Vidhya_Job_A_Thon/blob/main/Job%20A%20Thon.png" alt="18th rank" height="500" style="vertical-align:top; margin:4px">

# Thank you for visiting.
