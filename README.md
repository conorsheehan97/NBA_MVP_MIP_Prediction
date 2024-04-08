# NBA_MVP_DPOY_MIP_Prediction
In this project, we attempt to predict the NBA MVP, DPOY and Most Improved Player using a combination of Random Forest Regression and Statistical Analysis. 

This work involves using MVP & DPOY Share voting distributions over the last 10 years (obtained from https://www.basketball-reference.com/), which was sotred in a centralised SQLLite Database for ease of access. This data was used to create 10 Regression Decision Trees, and then ensembling their cumulative Share votes together (Random Forest) to determine who this seasons MVP & DPOY were. 

An amount of Exploratory Data Analysis was required initially to reduce the dataset, analyse what features correlated most strongly to a high MVP/DPOY share, and use these then on this seasons in-game player data. It was also fun to see what, statistically held the most relevance for MVP/DPOY voting. A comparison of the top 5 MVP's and DPOY's predicted for this season was then undertaken, and the order of the ranking was then evaluated against the bookmakers favourites. 

The final aspect of this project involved calculating the Most Improved Player. This section proved to be the most challenging. This required reducing the original dataset to only player data from the last 2 seasons, and only keeping rows that pertained to a players season summary statistics, and not their averages per team in a season they were traded. We then further reduced the data to only players who had played the average amount of MIP winner minutes over the last 5 seasons, and then unitised the data to ensure each feature had a fair contribution. We then gave each remaining player an 'Improvement Score', which measured statistically how a player has improved from the last season. Players were then ranked on this result. We then again compared our final results against the bookmakers odds!

Models used: Regression Decision Trees

Packages used: SQLLite3, Pandas, Numpy, Seaborn, Matplotlib, Scikitlearn, Joblib, Statistics, Math
