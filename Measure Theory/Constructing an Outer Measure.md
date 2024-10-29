#lemma
### Types
- `X` : Nonempty Set
- $\mathcal{E}$ subset of the [[Power Set]] of `X` containing $\varnothing$ and `X`
- $\mu:\mathcal{E} \to \left[ 0,+\infty \right]$ with $\mu \left( \varnothing \right) = 0$
### Statement
For any $A\in\mathcal{E}$, we define:
$$
\mu^*\left( A \right) = \inf\left\{\sum_{i=1}^\infty \mu \left( E_{i} \right)  :E_{i}\in\mathcal{E} \land A\subset\bigcup_{i=0}^\infty E_{i} \right\}  
$$
Then $\mu^*$ is an [[Outer Measure]].
### Proof
$\mu^*$ is well defined because for any $A$ in $P(X)$, there exists $\left\{ E_{i} \right\}_{i\in\mathbb{N}}$ such that $A\subset\bigcup\limits_{{i=0}}^\infty E_{i}$, as we can take $E_i = X, \forall i\in\mathbb{N}$. Now let's verify that it satisfies the conditions of an outer measure.
First, $\mu^*(\varnothing) = 0$, which is satisfied by taking $E_{i}=\varnothing, \forall i\in\mathbb{N}$.
Second, let $A \subset B \subset X$, then for any $\left\{ E_{i} \right\}$, if $B \subset \bigcup\limits_{i=0}^\infty E_{i}$, then the same can be said about $A$, so the set which we are taking the infimum of in the case of $\mu^*\left( B \right)$ is contained in that in the case of $\mu^*(A)$, so its infimum will be greater, thus $\mu^*(A) \le \mu^*(A)$.
Lastly, suppose $\left\{ A_{i} \right\}_{{i\in\mathbb{N}}}\subset P(X)$ and $\varepsilon > 0$. For each $i\in\mathbb{N}$, there exists $\left\{ E_{i,k} \right\}_{k\in\mathbb{N}}\subset\mathcal{E}$, such that $A_{i} \subset \bigcup\limits_{k=0}^\infty E_{i,k}$ and:
$$
\sum_{k=0}^\infty \mu \left( E_{i,k} \right) \le \mu^*\left( A_{i} \right) +\varepsilon 2^{-i}
$$
But then if $A=\bigcup\limits_{i=0}^\infty A_{i}$, we have $A\subset\bigcup\limits_{{i=0}}^\infty\bigcup\limits_{k=0}^\infty E_{i,k}$ and:
$$
\sum_{i=0}^\infty\sum_{k=0}^\infty \mu \left( E_{i,k} \right) \le\sum_{i=0}^\infty \mu^*\left( A_{i} \right) +\varepsilon
$$
Since $\varepsilon$ is arbitrary, we are done.