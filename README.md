# **Cryptocurrency Clustering Analysis**

This challenge applies clustering techniques to cryptocurrency market data to group cryptocurrencies based on their price change percentages over various time intervals. Principal Component Analysis (PCA) is also employed to reduce the dimensionality of the data while preserving most of the variance.

## **Overview**

The analysis follows these steps:

    Data Processing:
        Load the cryptocurrency market data.
        Normalize the data using Standard Scaler.

    K-Means Clustering:
        Apply K-Means clustering to identify groups of cryptocurrencies.
        Use the Elbow Method to determine the optimal number of clusters (k).

    Dimensionality Reduction:
        Perform PCA to reduce the data to three principal components.
        Compute the optimal k using the PCA-transformed data.

    Visualization:
        Plot clusters using scatter plots and observe grouping patterns.
        Analyze the feature weights for each principal component to determine key influences.

## **Findings**

    Optimal Number of Clusters:
        The Elbow Method indicates that the best value for k is 4. There is no difference in the best k value between using the original and PCA-transformed data.

    Explained Variance:
        The three principal components account for 89.5% of the total variance.

    Feature Influence:
        PCA1: At +0.59, price_change_percentage_200d has the strongest influence on PCA1.
        PCA2: At +0.56, price_change_percentage_30d has the strongest influence on PCA2.
        PCA3: At +0.79, price_change_percentage_7d has the strongest influence on PCA3.