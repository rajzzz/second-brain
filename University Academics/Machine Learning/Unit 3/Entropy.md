A measure of uncertainity or impurity in a dataset.
tells us how mixed the class labels are at a node.

- If all samples belong to one class → **Entropy = 0** (pure)
- If samples are evenly split across classes → **Entropy is maximum**

In [[Decision Tree]]s Entropy is used to compute [[Information gain]]:
- A Split is chosen to reduce the entropy the most. (gain the most information)n


$$ \Large Entropy(S) = -\sum p_i\log_2p_i$$
