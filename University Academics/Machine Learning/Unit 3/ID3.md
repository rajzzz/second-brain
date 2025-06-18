A [[Decision Tree]] algorithm used to classify data.
## Iterative Dichotomizer 3

Build the tree top-down:
- At each step choose the fature that gives maximum [[Information gain]].
- Continue Recursively unitl:
	- All instances are of the same class
	- Or no more features are left