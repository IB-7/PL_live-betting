# English Premier League sports-betting
<b>Author:</b> Isaac Barrera
![download.jpeg](./images/download.jpeg)

Task: Traditionally, sports-bettors have only relied on their own intuition and biases when placing their bets. This sports-betting model was made to assist bettors who gamble on the match results of the English Premier League as a hobby. Specifically, this model is meant to be utilized only in live-betting contexts. In other words, bets that are placed <i>during</i> a given match.

## Overview
Individual capstone project for Flatiron Data Science program. In this project, my goal was to find the best classification algorithm to predict the full-time result of a Premier League football/soccer match. I start by importing the necessary libraries, cleaning/preprocessing the data, and building a simple, baseline model. The goal of this project was to accurately classify the match result of an English Premier League (EPL) match to help sports-bettors make better decisions and increase their chances of winning the bets they place. That way, instead of the bettor losing money (which can often be the case), they make money instead. Through my analysis, I found that a logistic regression model performed the best in classifying the full-time result of an English Premier League match, achieving a 66% accuracy. The recommendation I have is to place bets on the team that is winning at half-time because these teams frequently go on to win the game at full-time.

## Business Problem
Bettors are looking for a model that can be used to help them make more informed decisions when placing their bets on Premier League matches. Traditionally, most sports-bettors have only relied on their own biases but with the help of data, their chances of winning their bets may increase. For general sports bettors who gamble as a hobby, this model should NOT be relied on as a source to make money.

## Data Understanding
The dataset used was from Kaggle. I used the match data from the start of the 2003/2004 season up to October of the 2021/2022 season. Most of the columns in the dataset are in-game statistics provided at the end of each match. In addition, the original dataset did not provide the betting favorite based on the moneyline. I used a sports-betting website to identify the moneyline favorite in each game and inserted this information into the dataset.

## Methods
For methods, I first cleaned the data by getting rid of columns and also dropping the irrelevant/redundant columns. I also performed scaling on the data before modeling so that all of the columns were on the same range/scale. Next, I used various classifier algorithms to be fitted and predict on the training and testing data, respectively. For a sports-betting context, the metric that I chose to focus on was accuracy. I used accuracy because for this problem, a false negative or a false positive have the same effect which is that the bet would be lost because it was incorrect. 

## Conclusion
Out of all the models that I tried on the dataset, the model that achieved the highest accuracy was a logistic regression model. A logistic regression model was able to acheive an accuracy of 66% on the test data. This model will allow bettors to identify the features of a Premier League match that are most determinant in the full-time match result. Using this analysis, bettors can wager their money based on data, not on their own intution and biases.

## For more information
Please review the full analysis in the Jupyter Notebook or the presentation

## Repository structure

├── images <- Includes images utilized in presentation

├── presentation.pdf <- PDF version of project presentation

├── README.md <- The top-level README for reviewers of this project, you are reading it right now

├── MVP.ipynb <- Minimum viable project jupyter notebook

├── notebook.pdf <- PDF version of minimum viable project jupyter notebook 

└── pl_results.xlsm <- Dataset
