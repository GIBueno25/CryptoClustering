# **Cryptocurrency Clustering Analysis**

This project applies clustering techniques to cryptocurrency market data to group cryptocurrencies based on their price change percentages over various time intervals. Principal Component Analysis (PCA) is also employed to reduce the dimensionality of the data while preserving most of the variance.

## **Overview**

The analysis follows these steps:

    Data Preprocessing:
        Load the cryptocurrency market data.
        Standardize the data using StandardScaler to normalize feature scales.

    K-Means Clustering:
        Apply K-Means clustering to identify groups of cryptocurrencies.
        Use the Elbow Method to determine the optimal number of clusters (k).

    Dimensionality Reduction:
        Perform PCA to reduce the data to three principal components.
        Recompute the optimal k using the PCA-transformed data.

    Visualization:
        Plot clusters using scatter plots to observe grouping patterns.
        Analyze the feature weights for each principal component to understand key influences.

## **Key Findings**

    Optimal Number of Clusters:
        The Elbow Method indicates the best value for k is 4, both for the original and PCA-transformed data.

    Explained Variance:
        The first three principal components account for 89.5% of the total variance, ensuring minimal information loss.

    Feature Influence:
        PCA1: Strongest influence from price_change_percentage_200d (+0.59).
        PCA2: Strongest influence from price_change_percentage_30d (+0.56).
        PCA3: Strongest influence from price_change_percentage_7d (+0.79).

