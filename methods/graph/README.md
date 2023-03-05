### Note
1. A graph: $G = (V, E)$
    - $V \in \mathcal{G}$: set of nodes
    - $E$: set of edges
2. A graph embedding-based recommendation model:

$$
  \text{arg}\min_{\Phi} \mathcal{E}_{\mathbf{\Theta}}\left(L\left(f(\Phi(v_i), \Phi(v_j)), p_{ij}\right)\right), \forall v_i, v_j \in \mathcal{G}
$$
  - $\Phi \in \mathcal{H}: \mathcal{G} \rightarrow \mathcal{R}^{n\times k}$
      - $\mathcal{H}$: hypothesis spae
      - $n = |V|$: the number of nodes
      - k: embedding size
  - $f$: $(\cdot, \cdot) \rightarrow \mathcal{R}$: similairy measurement
  - $L$: loss function
  - $\mathcal{E}$: objective function (expectation) with parameters $\mathbf{\Theta}$
  - $p_{ij}$: observed similairy between $v_i$ and $v_j$ 

