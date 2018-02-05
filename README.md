# Ames-House-price-prediction
Price prediction use linear models, the data is from Kaggle competetion in 2015.
The data has 79 explanatory variables describing aspects of homes in Ames, Iowa, the aim is to predict the final price of each home.
Solution Linear Regression model: Ridge L2, Lasso L1.
***************************************************************
The solution flow contains:
1. Read the data and dicovery
2. Feature engineering
 - Check outliers and remove them
 - Solving the missing value by fill with median or average or 0 depend on features
 - Make some numerical features to categories
 - Encode some categorical features as ordered numbers when there is information in the order
 - Create new features: simplifications of existing features, combinations of existing features
 - Find most important features relative to target, polynomials on the top 10 existing features
3. Select models
 - Default model with r2_scores, got 0.89 on test
 - Ridge(l2) model with r2_scores, got 0.905 with tuned alpha of 17.825
 - Lasso(l1) model with r2_scores, got 0.904 with tuned alpha of 160
***************************************************************
Observe performance on test data, the ridge model is best for price task.
