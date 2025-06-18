means that the algorithm **does not learn a model during training**.

Instead of learning a function or set of rules from the training data ahead of time (like Decision Trees or Logistic Regression do), a lazy learner:

- **Stores the entire training dataset as-is**
- **Defers computation until a query (test input) is made**
- **Does all the work during prediction time**

