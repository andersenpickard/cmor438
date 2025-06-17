## Linear Regression: MLB Pitcher Dataset

This project implements and analyzes Linear Regression applied to a dataset of MLB pitchers' expected statistics from Baseball Savant.

## What is Linear Regression?

Linear Regression is a method for evaluating the relationship between one dependent variable and one or more independent variables. 

In data science, Linear Regression not only allows you to analyze the strength of this relationship, but you can also use a linear fit to predict values that would follow that linear model.

In this project, I am using Linear Regression to analyze the relationship between traditional counting stats and modern expected stats for pitchers with at least 162 batters faced so far in 2025. In my process, I compared a wide variety of features - including counting stats to counting stats, expected stats to expected stats, and counting stats to expected stats. 

After examining trends through various comparisons, I applied the Linear Regression model to expected ERA and expected SLG, as I wanted to see whether expected ERA was a reliable predictor of expected SLG.

For context, in baseball, expected ERA is a way to remove defense and ballpark factors from the traditional ERA statistic, which puts a closer focus on a pitcher's actual, true performance. Expected SLG is a way to remove defense and ballpark factors from the traditional SLG statistic, which also puts a closer focus on a pitcher's actual, true performance.

## Dataset

I am using Baseball Savant's MLB pitcher dataset from their pitching leaderboard. This data is compiled by Major League Baseball and publicly available online for free. This dataset contains 677 observations with 17 features.

## Exploration

- xERA vs. xSLG
- xERA vs. xBA
- SLG/xSLG delta vs. BA/xBA delta
- ERA vs. xERA
- PA vs. BIP

- Final linear application: xERA vs. xSLG
