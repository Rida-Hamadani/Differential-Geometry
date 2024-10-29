#exercise
### Question
$\mathbb{R}^n$ is equipped with the [[Euclidean Topology]].
Let $u_{1},u_{2}, \cdots, u_{n}$ be [[measurable function]]s from a [[measurable space]] $X$ to $\mathbb{R}$, and let $\Phi : \mathbb{R}^n \to Y$ be [[Continuity|continuous]], where $Y$ is a [[topological space]]. Proof that $h : X \to Y$ defined as: $$h(x) = \Phi \left( u_{1}(x),u_{2}(x),\cdots, u_{n}(x) \right)$$
is measurable.
### Answer
Let $f:X\to \mathbb{R}^n$ be defined as $f\left( x \right)=\left( u_{1}(x),u_{2}(x),\cdots, u_{n}(x) \right)$, then $h = \Phi\circ f$, and using [[Composition of Continuous is Continuous]], it is enough to show to that $f$ is measurable.
Let $R=I_{1} \times I_{2} \times \cdots \times I_{n}$ where $I_{k}$ is an open interval in $\mathbb{R}$, such a set is called a [[rectangle]], we have:
$$
\begin{aligned}
f^{-1}\left( R \right) &= \left\{ x\in X, f\left( x \right)\in R  \right\}\\
&=\left\{ x\in X,u_{k}\left(x \right) \in I_{k}, \forall 1\le k\le n\right\}\\
&= \bigcap\limits_{k=1}^n\left\{ x\in X, u_{k}\left( x \right)\in I_{k}  \right\} \\
&= \bigcap\limits_{k=1}^n u_{k}^{-1}(I_{k}) 
\end{aligned}
$$
which is measurable, since each $u_{k}$ is measurable.
Using [[Open Sets in Euclidean Space are Unions of Rectangles]], any [[open set]] $U$ in $\mathbb{R}^n$ is countable union of rectangles, so $f^{-1}\left( U \right)$ is the countable union of pre-images of rectangles, which is measurable.
##### Source
Real and Complex Analysis - Walter Rudin - Chapter 1 Exercise 2