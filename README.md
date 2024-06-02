# NBA_MVP_MIP_Prediction
This project aims to predict the NBA MVP (Most Valuable Player) and MIP (Most Improved Player) using a combination of Random Forest Regression and Statistical Analysis.

## Overview
Using MVP Share voting distributions from the last 10 years, stored in a centralized SQLite database for ease of access, this data was used to create 10 Regression Decision Trees. The cumulative Share votes were ensembled (Random Forest) to determine this season's MVP.

An Exploratory Data Analysis (EDA) was initially conducted to reduce the dataset, analyze features correlating most strongly with high MVP/DPOY shares, and apply these findings to this season's in-game player data. This also provided insights into the statistical relevance of various features for MVP voting. A comparison of the top 5 MVP predictions for this season was then made against bookmakers' favorites.

The prediction for the Most Improved Player proved to be the most challenging part of this project. It required reducing the original dataset to player data from the last 2 seasons, retaining only season summary statistics, and filtering players by the average minutes played by MIP winners over the last 5 seasons. The data was then unitized to ensure each feature contributed fairly. Each player was given an 'Improvement Score,' which measured their statistical improvement from the previous season. Players were then ranked based on this score, and the results were compared against bookmakers' odds.

### Models Used
 - Regression Decision Trees
### Packages Used
 - SQLite3
 - Pandas
 - Numpy
 - Seaborn
 - Matplotlib
 - Scikit-learn
 - Joblib
 - Statistics
 - Math
### Data Source
 - Basketball Reference

## Conclusion
This project successfully demonstrates the use of Random Forest Regression and Statistical Analysis to predict the NBA MVP and Most Improved Player. By leveraging historical MVP Share voting data and player statistics, we were able to build robust models that provide insightful predictions for the current season.

Key highlights of this project include:

### Comprehensive Data Analysis: 
 - Through extensive Exploratory Data Analysis, we identified the most relevant features for predicting MVP and MIP, gaining valuable insights into the factors that influence these awards.

 ### Model Accuracy: 
  - The use of Regression Decision Trees and their ensembling into a Random Forest allowed for accurate predictions, validated by comparisons with bookmakers' odds.

### Challenges Overcome: 
 - The prediction of the Most Improved Player required meticulous data preprocessing and feature engineering, demonstrating the project's ability to handle complex data scenarios.

### Practical Applications: 
 - The methods and models developed in this project can be applied to other sports analytics problems, showcasing the versatility and power of machine learning in sports predictions.

This project not only provides a predictive framework for NBA awards but also serves as a template for future projects in sports analytics. We invite contributions and feedback to further refine and enhance this work.

Thank you for exploring this project, and we hope it offers valuable insights and tools for your own data science and machine learning endeavors in sports.
