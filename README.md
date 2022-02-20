# Datium-task
The steps taken to complte the task as below:
import the dataset and necessary libraries 
Drop columns that have more than 50 percent missing values 
splitting of the dataset to train and test set to avoid biasness or influence on test set
check for missing values and impute them based on mean and model for numerical and categorical respectively (perform the same imputation for test set)
perform some analytics based on the filled in values to see trends and insights
perform feature extraction separately for numerical and categorical (dummy variables). include variables that contributes to target value and drop the rest 
Drop features that correlates with each other for both numerical and categorical 
perform correlation check another time between numerical and categorical dummy variables and drop the correlated features
move on to machine learning:
4 models were created where two are parametric (linear and svr) and the other two are non-parametric (xgboost and random forest)
for linear and svr, check for normality of residuals once model is fitted and check overfit by getting r2score on train and test. Also need to scaling before apply Ml
for xgboost and random forest there is no need for scaling and model is compared based on the r2 score 
All 4 models were evaluated based on RMSE and r2score.
The best model was Xgboost


Some improvisation that can be done to existing model:
Perform imputation more thoroughly as there is alot of similarity between model and missing values such as warrantyKM and firstsrviceKM and many more instead of blindly choosing mean and mode. 
could drop outliers for some columns or at least limit them 
Could apply cross validation or split it 3 ways (train, val, test)
perform some gridsearch for hyperparameter tuning to increase scores of some models (eg: svr)
