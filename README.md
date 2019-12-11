# MSDS699 Final Project
## Project Goal
The Goal of the project is to use features of online news to predict the popularity (measured by number of shares).
## Data Description
URL: https://archive.ics.uci.edu/ml/datasets/online+news+popularity.  
  
This Dataset is from UCI Machine Learning Repository. It contains 59 features of and number of shares information for 39644 pieces of news originally collected from www.mashable.com.
## Modelling
### Regression
Initially, we used regression models to predict number of shares of a piece of news. All features except for news url and timedelta were included in the model and tandardScaler() was applied to numerical features for all the models except for random forest.  
We built a pipeline to train and compare 3 different algorithms:  
• Lasso Linear Regression  
• Ridge Linear Regression  
• Random Forest Regressor   
### Classification
Using regression models results in large errors, so we thought classification models may actually make more sense for this problem. We chose the median of numbers of shares as the threshold to classcify all the news as "popular" or "not popular".  
All features except for news url and timedelta were included in the model and StandardScaler() was applied to numerical features for all the models except for random forest.  
We built a pipeline to train and compare 4 different algorithms:  
• Logistic Regression  
• K-Nearest Neighbors  
• Naive Bayes  
• Random Forest classifier  
## Metrics
For the regression model, we chose Median Absolute Error as the North Star metric.  
For the classification model, we chose F1 score as our North Star metric.
## Conclusion
• Using f1-score as North Star Metric, Random Forest is the best model.  
• Recommendations for reporters and business entities:  
(1) Keywords are important.  
(2) Publication time matters.   
(3) Reference article with high popularity would help.
