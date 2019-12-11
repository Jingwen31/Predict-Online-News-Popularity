# MSDS699 Final Project
# Predicting Online News Popularity
### Xiao Chu, Zhentao Hou, Jingwen Yu
## Project Goal
The Goal of this project is to use features of online news to predict the popularity (measured by number of shares).
## Data Description
URL: https://archive.ics.uci.edu/ml/datasets/online+news+popularity.  
  
This dataset is from UCI Machine Learning Repository. It contains 59 features and number of shares information for 39644 pieces of news originally collected from www.mashable.com.
## Modeling
### Regression
Initially, we used regression models to predict the number of shares of a piece of news. All features except for news url and timedelta were included in the model and StandardScaler() was applied to numerical features for all models except for the random forest regressor.  
  
We built pipelines to train and compare 3 different algorithms: 
  
• Lasso Linear Regression  
• Ridge Linear Regression  
• Random Forest Regressor   
### Classification
Using regression models results in large errors, so we thought classification models may actually make more sense for this problem. We chose the median number of shares as the threshold to classify all the news as "popular" or "not popular". 
  
All features except for news url and timedelta were included in the model and StandardScaler() was applied to numerical features for all models except for the random forest classifier.  
  
We built pipelines to train and compare 4 different algorithms:  
  
• Logistic Regression  
• K-Nearest Neighbors  
• Naive Bayes  
• Random Forest Classifier  
## Metrics
For the regression model, we chose Median Absolute Error as the North Star metric.  
  
For the classification model, we chose F1 Score as the North Star metric.
## Conclusion
• Using F1 score as the North Star Metric, Random Forest is the best model.  
  
• Recommendations for reporters and business entities:  
  
(1) Keywords are important.  
(2) Publication time matters.   
(3) Referencing articles with high popularity would be helpful.
