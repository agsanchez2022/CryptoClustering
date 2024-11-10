# CryptoClustering

In this project, we apply unsupervised learning techniques to analyze cryptocurrency data, predict the impact of 24-hour or 7-day price changes, and use clustering to uncover hidden patterns. This includes using K-means clustering, Principal Component Analysis (PCA), and evaluating different clustering methods.

## Project Overview

This project includes the following steps:
1. **Data Preparation**: Load cryptocurrency market data and normalize using `StandardScaler()`.
2. **Elbow Method for K-means**: Identify the best value of `k` for clustering.
3. **K-means Clustering**: Perform clustering of cryptocurrencies and visualize the results.
4. **Principal Component Analysis (PCA)**: Optimize clusters using PCA to reduce feature dimensions.
5. **Cluster Optimization**: Evaluate clustering results with PCA reduced data.
6. **Comparative Analysis**: Compare clustering results using original data versus PCA data.

## Files

1. `Crypto_Clustering.ipynb`: Jupyter notebook containing the analysis and steps for clustering cryptocurrencies.
2. `crypto_market_data.csv`: The dataset containing cryptocurrency market data.

## Data Analysis Steps

### 1. Data Preparation
- Load the `crypto_market_data.csv` into a Pandas DataFrame.
- Normalize the data using `StandardScaler` to standardize features.

### 2. Finding the Best Value for k (Using Elbow Method)
- Run K-means clustering for different values of `k` (from 1 to 11).
- Plot inertia values to visually identify the optimal number of clusters.

### 3. K-means Clustering (Using Scaled Data)
- Use the best `k` value from the Elbow Method.
- Perform clustering on the scaled dataset and visualize using `hvPlot` with price changes.

### 4. Optimize Clusters with PCA
- Perform PCA to reduce the feature dimensions to 3 components.
- Visualize explained variance and cluster optimization using reduced features.

### 5. Clustering with PCA Data
- Reapply K-means clustering using the PCA-reduced dataset.
- Visualize clusters using `PC1` and `PC2`.

### 6. Visualizing and Comparing Results
- Use composite plots to compare elbow curves from original vs PCA data.
- Compare clustering results from both original and PCA data.






