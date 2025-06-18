- Initialize kkk random **medoids** m1,m2,...,mkm_1, m_2, ..., m_km1​,m2​,...,mk​
    
- Assign each point to the **nearest medoid**
- For each cluster, select the data point mj∈Cjm_j \in C_jmj​∈Cj​ that minimizes:
$$\Large {\sum_{x_i \in C_j} d(x_i, m_j)}$$
- Repeat until medoids do not change


- Robus to [[Outliers]]
- Can use both [[Manhattan-Distance]] and Euclidean Distance.