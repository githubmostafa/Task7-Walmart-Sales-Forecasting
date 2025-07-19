✅ Walmart Sales Forecasting
This repository contains a time series machine learning project that predicts weekly sales for Walmart stores using historical data.
The project includes data preprocessing, feature engineering, time-based modeling, model evaluation, and saving trained models.

📁 Dataset Source: Walmart Store Sales Forecasting (Kaggle)
📝 Description: Weekly sales data from multiple Walmart stores and departments
🎯 Target: Predict future weekly sales based on historical trends and external features

📊 Models Used and Compared

✅ Linear Regression

Basic regression using time-based and lag features

Evaluated with RMSE and MAE

Good baseline performance

✅ XGBoost Regressor with TimeSeriesSplit

Gradient boosting model trained with time-aware cross-validation

Handled temporal dependencies better than linear models

Outperformed Linear Regression in both RMSE and scatter plot visualizations

🛠️ Features

Data loading, merging, and cleaning

Feature engineering:

Time-based features: year, month, week

Lag features: lag_1, lag_2, lag_3

Rolling averages: rolling_mean_3

Exploratory data analysis

Seasonal decomposition using statsmodels

Regression modeling:

Linear Regression

XGBoost with TimeSeriesSplit

Model evaluation:

RMSE

MAE

Actual vs. Predicted plots

Model saving using .model and .json

📦 Requirements

pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
statsmodels

📈 Sample Results

Model: Linear Regression
RMSE: 5591.49
MAE: 1597.73

Model: XGBoost (CV=5)
RMSE: 4301.73

🧩 Visuals show improved accuracy and tighter clustering around the ideal line for XGBoost.

📊 Result Summary

Time-based features and lag features significantly improved predictions

XGBoost outperformed Linear Regression using temporal cross-validation

Seasonal decomposition revealed clear trends in sales for certain stores

All core and bonus tasks were successfully implemented

📌 License
This project is intended for educational and portfolio purposes only. Based on the Kaggle Walmart Forecasting competition dataset.

