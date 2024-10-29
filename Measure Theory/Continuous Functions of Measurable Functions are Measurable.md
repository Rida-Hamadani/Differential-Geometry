#lemma
### Types
- `X` : [[Measure Space]]
- `Y` `Z` : [[Topological Space]]
- $f : X \to Y$
- $g : Y \to Z$
### Statement
If $f$ is [[Measurable Function|measurable]] and $g$ is [[Continuity|continuous]], then $g \circ f$ is measurable.
### Proof
If $U$ is an [[open set]] in $Z$, then $g^{-1}\left( U \right)$ is open in $Y$, thus $f^{-1}\left( g^{-1} \left( U \right) \right)$ is [[Measurable Set]] in $X$, so $g\circ f$ is [[Measurable Function]].