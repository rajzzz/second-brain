## L1 Regularization
 - uses L1 regularization penalty.
- Adds the absolute value of the coeffecients to the cost functions:
$$ \Large {Penalty = \lambda \sum_{i=1}^n |w_i|}$$
- Lasso Regularization tends to shrink some of the coefficients to zero, effectively performing feature selection.
- Particularly useful when there is a large number of irrelevent [[Features]] in the in dataset.

#### Appllications:
- When feature selection is important, such as in genetics, economics and text data analysis.