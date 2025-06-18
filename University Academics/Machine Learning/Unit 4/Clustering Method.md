#### 1. Partitioning Methods:
- **Objective:** Partition the data into k clusters where each cluster is represented by a centroid.
- Example Algorithms:
	- [[K-Means]]: Minimizes the sum of squared distances between points and the clusters centroid.
	- [[K-Medoids]]: Similar to K-means but uses actual data points as centroids (more robust to noise)
- Simple and efficient for large data sets.
- Requires specifying number of clusters (k)
- Sensitive to outliers

#### 2. Heirarchical Methods
- **Objective** Build heirarchy of clusters using a tree-like structure called dendrogram.
- **Types:**
	- *Bottom-Up (Agglomerative):* Start with each data point as a cluster and merge them iteratively.
	- *Top-Down(Divisive):* Start with one cluster and split it iteratively.
- Does not require specifying the number of clusters
- Computationally Expensive for large datasets.

#### 3. Density-Based Methods:
- **Objective:** Identify clusters based on regions of high density
- Example Algorithms:
	- [[DBSCAN]] (Density-Based Spatial Clustering of Applications with Noise)
	- [[OPTICS]] (Ordering Points To Identify the Clustering Structure)
- Can handle noise and clusters of arbitraty shapes.
- Struggles with varying densities and high-dimensional data.
#### 4. Grid-based Methods:
- **Objective:** Divide the data space into a grid and perform clustering on the grid.
- Example algorithm:
	- [[STING]] (Statistical Information Grid):
- Efficient for large datasets.
- Sensitive to grid size.

#### 5. Model-Based Methods:
- **Objective:** Assume a model for each cluster and find the best fit for the data.
- Example Algorithms:
	- [[GMM]] (Gaussian Mixture Models)
	- [[Expectation-Maximization]]
- Flexibility in capturing clusters of different shapes and densities.
- Computationally expensive.