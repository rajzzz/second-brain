## (L2 Regularization)

- Includes a regulaization term (L2 penalty) to prevent [[Overfitting]]. 

- This term penalizes large coefficients by adding their squared values to the cost function.
$$ \Large {Penalty = \lambda \sum_{i=1}^{n}w^2_i}$$
- By this, ridge regression reduces the complexity of the model, leading to better generalization
#### Application:
- Commonly used when the number of features is large and there is [[multicollinearity]] among the features.
