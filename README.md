# Predicting Wins and Losses in the NFL

Our research’s goal is to predict the outcome of an NFL game. Given the NFL’s popularity coupled with the rising influence of regulated sports betting, a predictive model can be leveraged to gain an edge over sportsbooks. Building on FiveThirtyEight's methodology, we created three predictive algorithms, random forest, k-nearest neighbors, and logistic regression, to predict winners and losers. The study utilizes a dataset provided by FiveThirtyEight which features team Elo ratings and quarterback Elo ratings. Our findings reveal that all three models achieved accuracy scores around 65%, surpassing FiveThirtyEight's reported 64%. The models also had similar precision scores, hovering around 66%. The models performed better in predicting wins than losses, prompting consideration of potential biases. The models are considered successful. Dataset expansion to include other important factors could improve the models’ accuracy. 

There are 5 ipynb files; NFL_Preprocessing, NFL_RandomForest, NFL_KNN, NFL_Logistic_Regression, and NFL_Validation.

NFL_Preprocessing is not needed to run the other files. All of the preprocessing is stored in that file, and is present in the rest of the files. 

All that is needed to run the other four files, is to have the dataset in the project folder. Our dataset is called “nfl_elo.csv”, but the shortened one will be called “nfl_elo_shortened.csv”. In the second cell of all 5 files, there is a line of code that reads as “data = pd.read_csv(“nfl_elo.csv”, header=None, names=col_names)”. To run the notebook with the shortened dataset, change the highlighted portion and replace it with “nfl_elo_shortened.csv”, or replace the entire line with “data = pd.read_csv(“nfl_elo_shortened.csv”, header=None, names=col_names)”.

To ensure that there are no errors while running the code, start at the very first cell, and run the subsequent cells in order. 
