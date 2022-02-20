# Datium-task
The steps taken to complete the tasks are as below:\
1. import the dataset and necessary libraries\
2. Drop columns that have more than 50 percent missing values\
3. splitting of the dataset to train and test set to avoid biasness or influence on test set\
4. check for missing values and impute them based on mean and model for numerical and categorical respectively (perform the same imputation for test set)\
5. perform some analytics based on the filled in values to see trends and insights\
6. perform feature extraction separately for numerical and categorical (dummy variables). include variables that contributes to target value and drop the rest\
7. Drop features that correlates with each other for both numerical and categorical\ 
8. perform correlation check another time between numerical and categorical dummy variables and drop the correlated features\
  
Move on to machine learning:\
1. 4 models were created where two are parametric (linear and svr) and the other two are non-parametric (xgboost and random forest)\
2. for linear and svr, check for normality of residuals once model is fitted and check overfit by getting r2score on train and test. Also need to do scaling before applying regression\
3. for xgboost and random forest there is no need for scaling and model is compared based on the r2 score\ 
4. All 4 models were evaluated based on RMSE and r2score\
5. The best model was Xgboost\


Some improvisation that can be done to existing model:
1. Perform imputation more thoroughly as there are lots of similarity between model and missing features such as warrantyKM and firstsrviceKM and many more\ 
2. could drop outliers for some columns or at least limit them\ 
3. Could apply cross validation or split it 3 ways (train, val, test)\
4. perform some gridsearch for hyperparameter tuning to increase scores of some models (eg: svr)\
