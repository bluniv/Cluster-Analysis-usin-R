# Cluster Analysis using R


## Project Overview

This project involves a comprehensive analysis on cluster analysis techniques. The primary goal is to identify patterns, relationships, and distinctive groups within the dataset. The main steps and findings are summarized below.

## 1) Getting Data

The dataset utilized for this analysis is the Walmart sales dataset, a rich source of information encompassing sales figures, temperature records, and fuel prices. The dataset was obtained from <u>https://www.kaggle.com/datasets/yasserh/walmart-dataset</u>

## 2) Plotting of Data

To initiate the exploration of the dataset, a pair plot was generated. This multivariate visualization allowed a thorough examination of relationships between different variables. The pair plot aids in understanding potential correlations and distributions within the data.  Two specific scatter plots were created to delve deeper into the relationship between sales and key variables:

### Sales against Temperature

This scatter plot visualizes the impact of temperature on sales, helping to identify any discernible trends or patterns.

### Sales against Fuel Price

Examining the correlation between fuel prices and sales through this scatter plot provides insights into how fuel costs might influence consumer purchasing behavior.

## 3) Normalization of Data

Normalization is a crucial preprocessing step in cluster analysis. It ensures that variables with disparate scales do not unduly influence the clustering process. The `scale` function was applied to normalize the dataset, aligning variables on a comparable scale.

## 4) Distance Matrix

A distance matrix was computed using the normalized data. This matrix quantifies the dissimilarity between observations, serving as a foundation for subsequent hierarchical clustering.

distance = dist(norm)


## 5) Hierarchical Agglomerative Clustering

Hierarchical agglomerative clustering was conducted using the `hclust` function. The resulting dendrogram provides an intricate visualization of the hierarchical relationships between data points, revealing potential clusters.

## 6) Hierarchical Agglomerative Clustering with "Average" Linkage

The clustering process was repeated using "average" linkage, offering an alternative perspective on cluster structures within the dataset. The dendrogram resulting from this method provides additional insights into average linkage clustering.

## 7) Cluster Membership

Clusters were identified based on the hierarchical clustering dendrogram. This information was extracted, providing a foundation for subsequent cluster characterization.

## 8) Characterizing Clusters

To better understand the nature of each cluster, an in-depth analysis of cluster characteristics was performed. Mean values of each variable within clusters were examined, uncovering distinctive traits associated with each group.

## 9) Scree Plot

A scree plot was generated to facilitate the determination of an optimal number of clusters. This plot visualizes the variabilities within clusters, aiding in the selection of the most suitable number of clusters based on within-group sum of squares.

## 10) K-means Clustering

Finally, k-means clustering was employed to partition the data into distinct clusters. The insights gleaned from the scree plot guided the determination of the optimal number of clusters, contributing to a more nuanced understanding of the dataset.
