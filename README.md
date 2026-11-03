# Marketing and Sales: Simple Linear Regression

Simple linear regression on a marketing and sales dataset in Python, done as part of a Coursera data course. The notebook models how radio promotion budget relates to sales and checks the assumptions of linear regression.

## Notebook

* `simple_linear_regression.ipynb`: data exploration, cleaning, pairwise plots, an OLS model of sales on radio budget, and assumption checks

## What it covers

* Exploring the data and dropping rows with missing values
* Pairwise plots to check the linearity assumption
* Fitting an ordinary least squares (OLS) model with `statsmodels`
* Reading the model summary: intercept, slope, p-value and R-squared
* Checking assumptions with a regression plot, residual histogram, Q-Q plot and a plot of residuals against fitted values

## Key findings

* The data has 572 rows and 5 columns (TV, Radio, Social Media, Influencer and Sales), and three rows with missing values were dropped
* Radio and Sales have a roughly linear, positive relationship, with a correlation of about 0.87
* The fitted model is Sales = 8.17 * Radio + 41.53, with values in millions of dollars
* Each additional million dollars of radio promotion is associated with about 8.17 million dollars more sales on average
* The slope is statistically significant (p < 0.001), and R-squared is about 0.757, so radio budget explains roughly 76% of the variation in sales
* The residuals are approximately normal, show no clear pattern against the fitted values, and have a Durbin-Watson statistic of about 1.88, so the model assumptions hold
* This shows an association, not proof of cause, and the model uses a single predictor. A multiple regression adding TV, social media and influencer type is a sensible next step

## Tools

Python, pandas, seaborn, matplotlib, statsmodels, Jupyter Notebook

## Data

marketing_sales_data.csv
