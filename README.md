# Project Name
> A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file. The company is looking at prospective properties to buy to enter the market. A regression model is built using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.
The company wants to know:
* Which variables are significant in predicting the price of a house, and
* How well those variables describe the price of a house.



## Table of Contents
* Data Cleaning
* Feature Engineering
* * Transform ordered categorical variables to numeric
* * Combine different levels for categorical variables to linearize the relationship
* Exploratory Data Analysis
* Data Preparation
* * Dummy Variable creation
* Model Building and Evaluation
* Variable Importance

## Process Summary
* Simple Linear Regression is used to find a suitable model.
* Variable selection is done based on p values and VIF
* Lasso and Ridge regression is applied on the model thus selected
* Lasso regression is also evaluated for Feature reduction where feasible.
* 5 fold Cross Validation is used on train dataset is used to determine the optimum alpha parmeter. Coarse and fine tuning is performed.
* Train Test is split on 80:20 split
* 5 fold CV is only applied on Train dataset
* Using the optimum parameter ridge/lasso regression is fitted on the train data and also evaluated on the unseen test data.
* Model performance is evaluated on the unseen test data
* Variable importance for both Ridge/Lasso regression is evaluated using the magnitude of the coefficients. Higher magnitude implies high variable importance.
* Redidual Diagnostics are also performed to check for heteroscedasticity and normality of the residuals besides p value, F Statistic and VIF.

