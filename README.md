This project applies K-Means clustering to group cryptocurrencies based on their price change percentages. It also optimizes clustering using Principal Component Analysis (PCA) to reduce dimensionality while preserving variance.

Key Steps

Prepare the Data

  Load cryptocurrency market data from a CSV file.
  Normalize the data using StandardScaler().
  Create a DataFrame with the scaled data, using coin_id as the index.

Find the Optimal k (Elbow Method) - Scaled Data

  Compute inertia for k = 1 to 11.
  Plot an Elbow Curve using hvplot.
  Identify the best k value for clustering.

K-Means Clustering on Scaled Data

  Train a K-Means model with the best k value.
  Predict cluster labels and add them to the DataFrame.
  Visualize the clusters using a scatter plot (hvPlot).

Optimize Clustering with PCA

  Reduce the dataset to 3 principal components.
  Compute the explained variance.
  Create a new PCA-transformed DataFrame.

Find the Optimal k (Elbow Method) - PCA Data

  Repeat the elbow method on the PCA-transformed data.
  Compare the optimal k with the original scaled dataset.

K-Means Clustering on PCA Data

  Train K-Means on the PCA DataFrame.
  Predict cluster labels and add them to the DataFrame.
  Visualize the clusters using a scatter plot (hvPlot).

Analysis

  Compare the clusters before and after PCA.
  Discuss the impact of reducing features on clustering results.

