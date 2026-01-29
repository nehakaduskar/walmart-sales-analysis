# Walmart Sales Analysis Overview
This project analyzed historic Walmart sales data ranging from 2010 to 2012 across 45 stores and evaluated multiple regression models to predict weekly sales. The project combines data analysis, visualization, regression, and an [interactive Power BI dashboard](https://app.powerbi.com/reportEmbed?reportId=02ca9f1b-c422-4555-bb03-c869d0b739c6&autoAuth=true&ctid=44467e6f-462c-4ea2-823f-7800de5434e3). The dashboard contains information about sales trends based on stores, date, size, and type and also evaluated the linear regression performance.

# Data Preparation
* Merge datasets containing store size, features, and sales into one dataset
* Fill na values with 0 (markdown columns)
* Convert dates into time based features (year, month, week, day of week)
* one hot encode categorical variables

# Regression
Compared and implemented :
* Linear regression
* Elastic Net Regression
* Ridge Regression
* Lasso Regression
Models were evaluated on R^2 value, RMSE and inherent advantages and disadvantanges (multicollinearity, feature selection)

# Results
* Regularized regression did not yield a significantly stronger R^2 or RMSE
* Best R^2 = 0.66, best RMSE = 13.2K
* Moderate R^2 and high RMSE means model could not predict high variability in dataset
* LASSO identified subset of variables of uninfluential predictors by shriking coefficients to 0.

# Power BI Dashboard
Link: https://app.powerbi.com/reportEmbed?reportId=02ca9f1b-c422-4555-bb03-c869d0b739c6&autoAuth=true&ctid=44467e6f-462c-4ea2-823f-7800de5434e3
* Showcased trends over time, by size, holiday, and store type (A = large, B = Medium, C = Small)
* Evaluated linear regression model comparing actual vs predicted sales over time and residuals 
