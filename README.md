NYC Temperature Analysis

This repository contains a Python-based analysis of historical temperature data for New York City, covering the period from January 1895 to January 2018. The analysis involves data cleaning, exploratory data analysis (EDA), and the use of linear regression models to predict future temperatures.

Project Overview

The project involves analyzing historical temperature data to understand trends over time and predict future temperatures using a linear regression model. The dataset includes monthly average high temperatures and their anomalies from the long-term average.

Data

The dataset used in this analysis is ave_hi_nyc_jan_1895-2018.csv, which contains three columns:

Date: Year and month of the observation (e.g., 189501 for January 1895).
Temperature: The average high temperature for that month.
Anomaly: The deviation of the average high temperature from the long-term average.

Requirements

Python 3.x
Pandas
NumPy
Scikit-learn
Seaborn
Matplotlib

Results

The linear regression model shows a positive trend in average high temperatures in New York City over the analyzed period. The model predicts an average high temperature of approximately 39.83°F in January 2070.

training %	testing %	RMSE	comments

50	              50	4.55	a smaller training data leads to poorer performance

80	              20	4.01	better than the 50% split but not as good as the 90% split.

90	              10	3.67	has the lowest rmse because it has the highest training data

75	              25	4.16	split shows an RMSE of 4.16 which is slightly
                            worse than the 80% split but better than the 50% split.
