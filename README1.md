Public Transport Passenger Time-Series Analysis and Forecasting

This project focuses on end-to-end Time Series Exploratory Data Analysis (EDA), data preprocessing, seasonality and trend analysis, stationarity testing, outlier detection, and forecasting using multiple statistical models.
The dataset contains daily public transport passenger records and the goal is to understand the patterns and forecast future values.

Project Objectives

Perform complete EDA on a multi-column time-series dataset.

Explore trends, seasonality, cyclic patterns, and statistical properties.

Detect and handle outliers using techniques such as Winsorization.

Test stationarity using the Augmented Dickey-Fuller (ADF) test.

Build forecasting models such as:

ARIMA

SARIMA

Prophet

Compare forecast accuracy using MAE, RMSE, MAPE.

Provide insights that support decision-making for public transport management.

Technology Stack
Programming Language

Python 3.10+

Libraries Used
Category	Libraries
Data Handling	pandas, numpy
Visualization	matplotlib, seaborn
Time Series Analysis	statsmodels, pmdarima
Forecasting	Prophet
Outlier Handling	scipy (winsorize)
Environment	Google Colab, Jupyter Notebook
Why These Technologies Are Used
pandas and numpy

Used for efficient data loading, cleaning, transformation, and handling large time-series datasets.

matplotlib and seaborn

Used for visualizing:

trends

seasonality

correlations

boxplots for outlier detection
Visual insights are essential before forecasting.

statsmodels

Provides powerful statistical tools required for:

ADF test

Seasonal decomposition

ARIMA/SARIMA models

Autocorrelation (ACF) and Partial Autocorrelation (PACF) plots

These models are standard for classical forecasting and interpretability.

Prophet

Prophet handles:

strong seasonality

missing values

irregular intervals

automatic trend/seasonality detection
It is useful when dataset has multiple seasonal patterns.

scipy Winsorization

Used to cap extreme outliers when removing them would harm the time-series continuity.

Google Colab

Supports:

GPU/TPU (if needed)

Easy GitHub integration

Simple environment setup

Dataset Description

The dataset contains daily passenger counts across different zones.
Columns include:

date

power_consumption_zone2 (example column used for EDA)

other zone columns (up to 9) depending on dataset

The target for forecasting is each individual time-series column, meaning that every zone can be forecasted separately.

Workflow and Methodology
1. Load and Clean Data

Convert the date column to datetime type.

Sort the dataset by date.

Check for missing values.

Remove or impute missing values if required.

2. Exploratory Data Analysis

Line plots for trend identification.

Seasonal decomposition into trend, seasonality, residual.

Correlation between columns.

Resampling (daily, weekly, monthly averages).

3. Outlier Detection

Boxplots for each column.

Calculation of IQR.

Winsorization applied when needed.

4. Stationarity Testing

Perform ADF test.

If data is non-stationary, apply differencing or transformations.

5. Model Building
ARIMA

Used when:

Data has no strong seasonal component.

Data becomes stationary after differencing.

SARIMA

Used when:

Dataset contains clear seasonality (weekly/monthly patterns).

Prophet

Used when:

Multiple seasonalities are present.

Trend and holiday effects matter.

6. Forecast Evaluation

MAE

RMSE

MAPE

Time-based validation (rolling forecast origin)

7. Final Forecasting

Produce future predictions for:

7-day

30-day

90-day


Key Insights You Can Learn From This Project

How real-world time-series behaves across zones.

Effect of seasonality on transport passenger load.

Impact of trends (increasing or decreasing usage).

How outliers affect forecasting and how to handle them.

Difference between ARIMA, SARIMA, and Prophet.

How to evaluate forecasting models.
