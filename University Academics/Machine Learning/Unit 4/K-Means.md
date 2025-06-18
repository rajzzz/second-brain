Partition n data points into $k$ clusters $C1,C2,...,Ck$​ such that the **total within-cluster variance** is minimized.

**Steps:**

1. Initialize `k` random centroids
2. Assign each point to the nearest centroid:
	- $d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$
3. Recompute centroids as the **mean** of assigned points
	- $\mu_j = \frac{1}{|C_j|} \sum_{x_i \in C_j} x_i$
4. Repeat until centroids don't change

- Sensitive to outliers
- only uses Euclidean distance.