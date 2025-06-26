## Random Forests: NFL Quarterback EPA Data Set

This project implements and analyzes Random Forests applied to a dataset of NFL quarterback EPA totals from Sumer Sports.

## What are Random Forests?

Random forests are a machine learning method used for classification and regression. The model builds a "forest" of several decision trees and combines their outputs to produce a more accurate and stable prediction. Each tree is trained on a randomly selected subset of the training data and considers a random subset of features when making splits. A random forest averages the predictions of all its trees. 

This approach helps reduce overfitting. Because each tree sees different training samples and feature combinations, their individual errors tend to cancel out when averaged. Random forest models are also robust, making them less sensitive to small outliers in the dataset.

Another strength of random forests is their flexibility. They can handle numerical and categorical variables and can function despite missing values. They also provide useful estimates of feature importance to identify which variables have the greatest impact on specific predictions. 

Generally, random forests do perform well without requiring significant hyperparameter tuning.

![Random Forests Visualization](forest_viz.png)
_Image Credit: Roi Yehoshua / Medium_

## Dataset

I am using Sumer Sports' 2024 quarterback dataset from their player statistics dashboard. This data is compiled by Sumer Sports and publicly available online for free. This dataset contains 77 observations with 18 features. Columns including counting stats and expected stats.

## Exploration

The features used for this exploration are: 'Scramble %', 'Sack %', 'ADoT', 'Pass Yards', 'Pass TD', 'INT', 'YPA'
