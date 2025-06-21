## Neural Networks: MLB Individual Game Data Set

This project implements and analyzes Neural Networks applied to a dataset of MLB individual game events from Baseball Savant.

## What are Neural Networks?

Logistic regression is a supervised machine learning algorithm that predicts the probability of a certain outcome through binary classification. The model determines probability through just two possible outcomes: 1/true, 2/false. 

By classifying every outcome as either true or false, logistic regression provides a clear prediction (essentially a yes/no or true/false) rather than a scale for a certain outcome. For example, if a student developed a logistic regression model to determine the probability of them being admitted into a certain college, they would receive a clear "yes" or "no" answer rather than an interpretable probability, like "78%."

The equation for logistic regression with one feature is:

![Logsitic Regression](log_reg_fun.png)

The equation for logistic regression with multiple features is:

![Multiple Logistic Regression](multiple_log_eqn.png)

Logistic regression works best when the data in the dataset are linearly separable, which is the case with the example shown in this section. In my implementation of logistic regression here, I am analyzing a variety of features to predict whether the MLB players in the dataset will be classified as a power hitter. (For the sake of this implementation, I am classifying a "power hitter" as a .450+ slugging percentage.) This works because the outcome is going to be a binary observation. Rather than predicting their exact slugging percentage, I am predicting whether their status as a power hitter is "true" or "false."

## Dataset

I am using Baseball Savant's game dataset from their direct gameday link for the Cubs vs. Mariners game on June 20, 2025. This data is compiled by Major League Baseball and publicly available online for free. This dataset contains 58 observations with 12 features.

## Exploration

The features used for this logistic regression include exit velocity, launch angle, hit distance, bat speed, pitch velocity, and expected batting average.
