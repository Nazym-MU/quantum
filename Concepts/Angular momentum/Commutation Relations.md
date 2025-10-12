$$[\hat{J}_x, \hat{J}_y] = i\hbar\hat{J}_z \qquad [\hat{J}_y, \hat{J}_z] = i\hbar\hat{J}_x \qquad [\hat{J}_z, \hat{J}_x] = i\hbar\hat{J}_y$$
Cyclic Pattern: $[J_i, J_j] = i\hbar ε_{ijk} J_k$
where $ε_ijk$ is the Levi-Civita symbol (cyclic permutations give +1, anticyclic give -1).
## Physical Interpretation
**Components don't commute** → cannot simultaneously measure different components exactly.
- Measuring $S_z$ destroys information about $S_x$
- States are either $S_z$ eigenstates OR $S_x$ eigenstates, not both
## J² Commutes with Components
$$[\hat{J}^2, \hat{J}_x] = 0 \qquad [\hat{J}^2, \hat{J}_y] = 0 \qquad [\hat{J}^2, \hat{J}_z] = 0$$

where $\hat{J}^2 = \hat{J}_x^2 + \hat{J}_y^2 + \hat{J}_z^2$
- Derivation: [[Commutator of J**2 with J_z]]
- Consequence: Simultaneous Eigenstates: 
$$\hat{J}^2|j,m\rangle = j(j+1)\hbar^2|j,m\rangle \qquad \hat{J}_z|j,m\rangle = m\hbar|j,m\rangle$$

We can know both:
- Total angular momentum magnitude: $|\vec{J}| = \hbar\sqrt{j(j+1)}$
- z-component: $J_z = mℏ$
But NOT the x or y components simultaneously.
## Comparison: Two-Particle Systems
For two particles, individual operators commute:
$$[\hat{S}_{1i}, \hat{S}_{2j}] = 0$$
But components of each particle still don't commute with themselves:
$$[\hat{S}_{1x}, \hat{S}_{1y}] = i\hbar\hat{S}_{1z}$$
## Related
- [[Commutators]]
- [[Raising and Lowering Operators]]
- [[Compatible and Incompatible Observables]]