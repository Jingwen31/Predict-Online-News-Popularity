# MSDS699 Final Project
## Project Goal
The Goal of the project is to use features of online news to predict the popularity (measured by number of shares).
## Data Description
URL: https://archive.ics.uci.edu/ml/datasets/online+news+popularity.  
  
This Dataset is from UCI Machine Learning Repository. It contains 59 features of and number of shares information for 39644 pieces of news originally collected from www.mashable.com.
## Modelling
### Regression
Initially, we used regression models to predict number of shares of a piece of news. All features except for news url and timedelta were included in the model and tandardScaler() was applied to numerical features.  
We built a pipeline to train and evaluate 3 different algorithms:  
• Lasso Linear Regression
• Ridge Linear Regression
• Random Forest Regressor
