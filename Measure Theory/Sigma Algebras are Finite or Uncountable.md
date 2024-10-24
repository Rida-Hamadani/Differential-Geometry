#exercise
### Question
Prove that every [[Sigma Algebra]] is either finite or un[[countable]]. 
### Answer
Let `X` be a set, then if it is finite, every sigma algebra over it is finite. Assume it is infinite, we will show that a sigma algebra $\Sigma$ over `X` has to be uncountable. Assume $\Sigma$ is [[countable]].

The proof is divided into 4 steps:
1. Prove there exists an infinite family $S$ of disjoint [[measurable set]]s in $\Sigma$. It is countable because it is a subset of $\Sigma$, which is countable.
2. Different subsets of $S$ will give different unions since they are disjoint. These unions are contained in $\Sigma$ as they are countable unions due to $S$ being countable.
3. As each element of the [[power set]] of $S$ is the union of elements in $S$, it belongs to $\Sigma$, hence $\mathcal{P}\left( S \right)\subset\Sigma$.
4. The power set of an infinite set is uncountable, therefore $\Sigma$ is uncountable.
Now all left to prove step 1 and the proof will follow.
For every $x\in X$, let $S_{x}=\bigcap\limits_{x\in A}A$, the intersection of all [[measurable set]]s containing $x$. First, we will show that the elements of $S=\left\{ S_{x}, x\in X \right\}$ are disjoint. That is if $S_{x} \cap S_{y}\ne\varnothing$, then $S_{x} = S_{y}$.
Let $z\in S_{x}\cap S_{y}$, then $S_{z}\subset S_{x}\cap S_{y}$ by definition. So $S_{z}\subset S_{x}$ and $S_{z} \subset S_{y}$.
Suppose $x\not\in S_{z}$, then $x\in S_{x}-S_{z}$, but $S_{x}-S_{z}=S_{x}\cap \overline{S_{z}}$ is a measurable set containing $x$, so $S_{x}\subset S_{x}-S_{z}$, so $S_{z} = \varnothing$, a contradiction. Hence $x\in S_{z}$. Same logic leads to $y \in S_{z}$ too. By definition of $S_{x}$, this means $S_{x}\subset S_{z}$, so $S_{x} = S_{z}$. Similarly for $y$. So, $S_{x} = S_{y}$.
For each measurable set $E$ of $X$, $E = \bigcup\limits_{x\in E}E\cap S_{x}=\bigcup\limits_{{x\in E}}S_{x}$. $E$ is contained in this union because for every $x \in E, x \in S_x$. Suppose $x$ is an element of this union, then as the sets of $S$ are disjoint, it belongs to a specific $S_{x}=E\cap S_{x}$, thus it is contained in $E$.
Thus if $S$ is finite, every set of $\Sigma$ is the union of elements of $S$, which belongs to $\mathcal{P}\left( S \right)$, which is also finite, so $\Sigma$ would be finite, contradiction. 
##### Source
Real and Complex Analysis - Walter Rudin - Chapter 1 Exercise 1