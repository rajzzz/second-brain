A hidden Markov Model is a [[Statistical Models]] where:
- The system is modeled as a [[Markov-Process]] with hidden states.
- We observe outputs, but not the internal state directly.

Imagine trying to guess the **weather** (sunny, rainy, etc.) based on whether someone is **carrying an umbrella**.  
You **observe** the umbrella, but the **actual weather is hidden**.

$States: S = \{s_1, s_2, ..., s_N\}$
$Observations: O = \{o_1, o_2, ..., o_T\}$
$Transition matrix: A = [a_{ij}],\quad a_{ij} = P(s_j \mid s_i)$
$Emission matrix: B = [b_j(k)],\quad b_j(k) = P(o_k \mid s_j)$
$Initial distribution: \pi = [\pi_i],\quad \pi_i = P(s_i \text{ at } t=1)$

#### Applications:
- Speech recognition
- Stock price modelling