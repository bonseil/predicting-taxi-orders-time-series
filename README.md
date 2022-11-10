# predicting-taxi-orders-time-series

## Overview
Sweet Lift Taxi company has collected historical data on taxi orders at airports. To attract more drivers during peak hours, we need to predict the amount of taxi orders for the next hour. Let's build a model for such a prediction.

## Results

Analyizing the data we reached some very surprising insights. In the end, eXtreme Gradient Boosting proved to be the best suited for this job, with a very good RMSE score. 

## Steps in analysis

    Opening the data file and studing the general information
    Resampling the Time Series into hourly and daily intervals
    Analyzing the data; identifying the trend, seasonality and residuals
    Using the Dickey-Fuller test to verify if the series is stationary
      Surprisingly, even though the data appears to have a growing trend this is **not** a statistical significant increase.
      This realization has a big impact in our analysis
    Creating multiple features out of the given data
    Building several ML models and choosing the one with the best results.
    General conclusion

## Data description

    datetime - Date and time in intervals of 10 minutes
    num_orders - Number of orders in the 10 minute interval
