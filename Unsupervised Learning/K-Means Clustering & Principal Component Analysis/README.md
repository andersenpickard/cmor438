## K-Means Clustering and Principal Component Analysis: MLB Pitcher Dataset

This project implements K-Means Clustering and Principal Component Analysis applied to a dataset of MLB pitcher statistics from Baseball Savant.

## What is K-Means Clustering?

K-Means Clustering is an unsupervised machine learning algorithm that clusters data points into subgroups based on existing similarities. K-Means Clustering initializes a specified number of cluster centers and then assigns each data point to the nearest cluster center. After assigning points, the cluster centers are recalculated as the mean of all points inside that specific cluster. This process repeats until the clusters no longer change significantly.

The purpose of K-Means Clustering is to uncover hidden patterns that may not have previously been observed, either within the dataset or to the naked eye. It implements a technical process to distinctly cluster and group data points. Because of this, K-Means is especially useful when dealing with large datasets where manual labeling or inspection is not feasible. 

One drawback to K-Means Clustering is that it assumes clusters are equally sized and it is sensitive to outliers. This is why we implement the elbow method and silhouette score to determine the optimal K number of clusters for meaningful and interpretable clustering.

In my project, I am also including Principal Component Analysis. PCA can be looped into K-Means Clustering for visualization purposes, which is what I'm doing here. Whereas clustering is done in full-dimensional space, PCA helps project the results in 2D or 3D so that the clusters can be visualized clearly, as seen in my scatter plot with background regions.

![K-Means Clustering Visualization](kmeans_viz.png)
_Image Credit: Pranshu Sharma_

## What is Principal Component Analysis?

Principal Component Analysis (PCA) is a statistical process that simplifies datasets by reducing their dimensionality while preserving variance. It transforms the original features into a new set of uncorrelated variables called principal components. 

PCA is especially useful when working with datasets that have many variables because it can reveal patterns and underlying structures that might not be apparent in the raw data, especially to the basic human eye during a simple observation.

PCA effectively identifies eigenvectors in which data varies the most. These eigenvectors correspond to the axes of a new coordinate system, with the first principal component capturing the most variance, and so on. These components are computed from the eigenvectors of the data’s covariance matrix and the amount of variance captured by each component is indicated by its corresponding eigenvalue. 

PCA is commonly used in exploratory data analysis and image compression, such as what I'm doing here by using PCA as a complementary means of analysis. In this example, I am using PCA to assist with adding colors and background to the clustering process within my K-Means Clustering implementation.

## Dataset

I am using Baseball Savant's pitchers dataset from their custom leaderboards tool. All data was accumulated between Opening Day and the morning of June 26, 2025. This data is compiled by Baseball Savant and is publicly available online for free. This dataset contains 119 observations with 10 features. Columns include five rate stats regarding pitch location and result. 

## Exploration

I have selected five features that adequately contextualize a pitcher's performance over the course of the season. For all five, a greater positive percentage is better for the pitcher, and a lower positive percentage is worse for the pitcher. The percentages all relate to a pitcher's ability to induce weak contact and get results in/out of the zone. 

The features used for this exploration are: 'poorlyweak_percent', 'in_zone_percent', 'z_swing_percent', 'oz_swing_percent', 'whiff_percent'
