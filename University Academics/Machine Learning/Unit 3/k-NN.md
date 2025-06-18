k-NN is a [lazy](Lazy-Learning.md) and learning algorithm that **classifies a data point based on the majority label of its k nearest neighbors** in the feature space.

#### Steps in k-NN Algorithm
1. Choose the number of neighbours k.
2. Calculate the distance between the query point and all other poiints.
3. Sort and find k nearest
4. Assign the most frequent class label.

### Advantages:
* Simple and Intuitive.
* No training time.
* Works well with small datasets.

##### Disadvantages:
* Computationally expensive for large datasets.
* Sensitive to irrelevant features and feature scaling.
* Does not work well with high-dimensional data.
