# Task_kovai_co

 *Project Title*

Daily Public Transport Passenger Journey Analysis

 *Dataset*

File: Daily_Public_Transport_Passenger_Journeys_by_Service_Type_20250603.csv
This dataset contains daily passenger counts for different transport services:

->Local Route

->Light Rail

->Peak Service

->Rapid Route

->School

->Other (contains some missing values)

->Objective

To understand the travel patterns and build a time-series forecasting model (ARIMA/SARIMA) to predict future passenger journeys.

 *Work Done*

->Loaded and cleaned the dataset

->Converted Date column to datetime

->Identified missing values (20 in “Other”)

->Performed EDA (trend, pattern, comparison)

->Checked stationarity using ADF Test

->Applied differencing to make series stationary

->Built ARIMA/SARIMA forecasting models

Plotted forecast results

  *Key Insights*

->Passenger counts show clear daily and seasonal patterns

->Light Rail and Rapid Route have consistent high usage

->SARIMA performed better for forecasting than ARIMA

->Missing values handled without affecting trend

 *Output*

->Trend graphs

->Seasonal analysis

->Forecast for upcoming days
