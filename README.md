# Market Segmentation Notebook

This notebook performs market segmentation using K-means clustering, PCA, and autoencoder methods on sales data.

## Libraries Used

- Pandas
- Numpy
- Seaborn
- Matplotlib.pyplot
- Tensorflow.keras
- Sklearn.preprocessing
- Sklearn.cluster
- Sklearn.decomposition
- Sklearn.metrics
- Plotly.express
- Plotly.graph_objects

## Data Cleaning

Data Source : <a href="https://www.kaggle.com/kyanyoga/sample-sales-data">Kaggle</a>

The notebook performs simple data cleaning by dropping null columns and converting the ORDERDATE column to datetime format.

## Explanatory Data Analysis

The notebook performs the following steps for Exploratory Data Analysis:

## Visualizing the count of column items.

- Performing One Hot encoding to all categorical columns.
- Grouping data by order date to perform further analysis.
- Calculating Correlation Matrix.
- Plotting distplots.
- Visualizing the relationship between variables using pairplots.

## Market Segmentation

The notebook performs market segmentation using the following steps:

1. Fit K-means Clustering Model
   - Scale the data.
   - Find the optimal number of clusters using the elbow method.
   - Fit the K-means clustering model using the optimal number clusters (k).
2. Apply Principle Component Analysis
   - Visualize the results.
3. Perform Dimensionality Reduction using the Autoencoder
   - Create an autoencoder model using Keras API.
   - Fit and train the autoencoder model.
   - Use the bottleneck layer (after down-scaling layers and before up-scaling layers) to encode the sales dataframe.
   - Use the elbow method to find the optimal number of clusters.
   - Fit the encoded sales dataframe using K-means clustering model with the optimal number of clusters.
   - Apply Principle Component Analysis and visualize the results.
