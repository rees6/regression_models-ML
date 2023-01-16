# regression_models-ML
different types regression model from scratch (linear , lasso, ridge, multiple) for reference

# linear regression
description: fitting a linear model into the dataset (best fit line) that is used for predicting the output.
supervised model - so dataset must contain lable to train
general steps to apply linear regression model:
1. split the dataset into predictor (y) or dependent variable and input (X) independent variable.
2. from sklearn linear_model library apply linear regression directly passing the parameters
3. calculate the cost function or mean_square_error or mean_absolute_error for the model created. using crossvalidation orGridSearchCV available in model_selection in sklearn.
4. find the best fit model ~ the model with least error is the best model

linear model equation
![Picture1](https://user-images.githubusercontent.com/80048690/212714232-aae3ed21-5fb6-4f02-9fbf-2a7cdee469b5.png)

general cost function or distance formula between expected and actual output

![cost func](https://user-images.githubusercontent.com/80048690/212715075-644e3e0b-ae62-4036-ba82-b7a750c4ba03.png)


# ridge regression 
description: when linear model dosent fit and produce overfit or underfit results, ridge and lasso is a regularised version of linear regression model.
general steps to apply ridge regression model:
1. it follows the formula of L2 regularization
2. used if data contains more outliers (or) cause overfit or underfit (or) has 100% performance with training dataset but worst performance with test data set.
3. split the dataset into dependent and independent variables
4. from sklearn linear_model import ridge and pass the input parameters
5. calculate cost function to find best fit

rigde model equation

![ridge](https://user-images.githubusercontent.com/80048690/212715113-1c1f0464-f486-4de0-b874-be667a9153bf.png)

general cost function + lambda parameter squared is L2

![l2](https://user-images.githubusercontent.com/80048690/212715229-9813bf27-83c4-46d5-b981-bd6cb9b273ba.png)


# Lasso regression
description: similar to ridge but use the formula of L1 regularization technique (refer the formula for better understanding)
general steps to apply Lasso regression:
1. split the data
2. from sklearn under linear_model import Lasso, pass parameters
3. calculate cost functions find best  model

lasso model equation

![lasso](https://user-images.githubusercontent.com/80048690/212715417-7e85db21-3e24-46bd-9b7d-39d87628ea72.png)

general cost function + lambda parameter squared is L1

![L1](https://user-images.githubusercontent.com/80048690/212715427-caec4193-6400-49fd-9fa6-afb8fdf5d6ed.png)


# multiple regression
description: instead of 1 predictor variable and 1 independent variable multiple regression has many independent variable and only one dependent  or predictor variable. (ie. many X and 1 Y hence slight change in same formula of line equation)
general steps to apply Multiple regression
1. use same model as linear regression
2. from sklearn under linear_model import LinearRegression
3. while splitting dataset use iloc and slice many feature with x and output with y
4. many features - independent variable / output - predictor or dependent variable
5. find costfunction or score and get best fit.

multiple regression model equation


![multiple regression](https://user-images.githubusercontent.com/80048690/212715448-0029441a-ded1-4aea-87ef-b571caa4aec6.png)

