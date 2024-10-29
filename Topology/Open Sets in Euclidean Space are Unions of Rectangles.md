#lemma
### Types
- `n` : $\mathbb{N}$
### Statement
Let $U$ be an [[open set]] in the [[Euclidean Topology]] of $\mathbb{R}^n$, then it is the [[countable]] union of [[rectangle]]s.
### Proof
Let $U$ be an [[open set]] of $\mathbb{R}^n$, and $x \in U$. As $U$ is the union of balls (by definition of Euclidean topology), let $B(x, r)$ be an open ball around $x$ where $r > 0$, and let $R_{x}$ be a rectangle such that the endpoints of its intervals are rational, and that it is contained in $B(x,r)$.
As $R_{x} \subset U, \forall x\in U$, then $\bigcup\limits_{x\in U} R_{x} \subset U$. Now if $x \in U$, then $x\in R_{x}\subset\bigcup\limits_{x\in U} R_{x}$, so $U = \bigcup\limits_{x\in U} R_{x}$.
There is a [[countable]] number of $R_{x}$'s, as the number of possible endpoints to choose from is [[countable]]. 