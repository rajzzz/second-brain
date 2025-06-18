Removes parts of [[Decision Tree]] that do not improve the model, helping reduce [[Overfitting]] and model size.
#### Pre-Pruning:
- Set constraints before training:
	- Max Depth
	- Min samples per node
	- Min Information gain
- We only need to split the data if it imporves the model.

- might stop too early (risks underfitting)
- Faster than Post.

#### Post Pruning (reduced error pruning):
1. Build full Decision Tree
2. Use validation set to evaluate subtrees
3. Remove branches that do not improve accuracy

- Slower, happens after full tree is grown.