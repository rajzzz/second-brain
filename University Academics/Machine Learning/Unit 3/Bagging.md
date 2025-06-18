### **Bootstrap Aggregating**

An [[Ensemble Learning]] technique where:
- Multiple [[Bootstrap samples]] are drawn from the dataset (random sampling with replacement).
- A model is trained on each sample
- Final O/p

#### Why it works:
- By training on different samples the individual models become diverse.
- Averaging their predictions reduces variance without Increasing [bias](Algorithmic-Bias).

#### Example:
- [[Random Forests]]