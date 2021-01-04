# NHL_Points_Modelling
Using data from NHL API to analyze player statistics and model player points/game using XGBoost

Quick project to try out XGBoost models and see if I can beat my friends in our fantasy draft. I decided to see how accurate I could predict the 2019-2020 points/game of players in the NHL based on the players performance in the last 4 seasons and other basic info like Age, position, and nationality. I removed Goaltenders and players who have not played at least 5 games in each of the previous 4 seasons. After gathering the data into a dataframe I do some quick analysis of the data, create some features for the training, and scale the data.

I trained a Linear Regression model from SKLearn, XGBoost Tree model, and XGBoost Linear model. I used Grid search cross validation to optimize the hyperparamters of the XGBoost Tree model. I found the best performance with the XGBoost Linear model (Mean Aboslute Error in predicting points per game of 0.121), although all models performed very similarly, I suspect due to the small dataset size.
