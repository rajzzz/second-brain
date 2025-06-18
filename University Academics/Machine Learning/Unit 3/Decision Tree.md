
#### Steps:
1. Start with all data at the root node.
2. For each feature, calculate a splitting score (like [[Information gain]].
3. Chosse the best split (feature + value)
4. Split the data into child nodes.
5. Repeat Steps 2-4 for each child node.
6. Stop when:
	1. All data in a node belongs to the same class
	2. Max depth is reached
	3. Min number of samples per node is reached

- Easy to understand and visualize
- Handles both numerical and categorical data