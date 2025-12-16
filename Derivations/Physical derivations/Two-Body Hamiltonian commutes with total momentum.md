$$[Ĥ, \hat T_1(a)\hat T_2(a)] = 0$$

where $\hat H = \frac{P̂_1^2}{2m_1} + \frac{P̂_2^2}{2m_2} + V(|\hat r_1 - \hat r_2|)$

It's sufficient to show operators commute when acting on arbitrary two-particle position state |r₁, r₂⟩, since any state can be expanded in this basis.
## Action on Potential Energy

$$
\hat T_1(a)\hat T_2(a)V(|\hat r_1 - \hat r_2|)\,|r_1, r_2\rangle
$$
$$
= \hat T_1(a)\hat T_2(a)V(|r_1 - r_2|)\,|r_1, r_2\rangle
$$
$$
= V(|r_1 - r_2|)\,\hat T_1(a)\hat T_2(a)|r_1, r_2\rangle
$$
$$
= V(|r_1 - r_2|)\,|r_1 + a, r_2 + a\rangle
$$

After translation, position eigenvalues become:
- $\,\hat r_1|r_1 + a, r_2 + a\rangle = (r_1 + a)|r_1 + a, r_2 + a\rangle$
- $\,\hat r_2|r_1 + a, r_2 + a\rangle = (r_2 + a)|r_1 + a, r_2 + a\rangle$
Therefore:
$$
|(r_1 + a) - (r_2 + a)| = |r_1 - r_2|
$$

Distance unchanged.
$$
V(|r_1 - r_2|)\,|r_1 + a, r_2 + a\rangle
= V(|\hat r_1 - \hat r_2|)\,\hat T_1(a)\hat T_2(a)|r_1, r_2\rangle
$$
## Action on Kinetic Energy
From the form
$$
\hat T_1(a)\hat T_2(a) = e^{-i(\hat P_1 + \hat P_2)\cdot a/\hbar},
$$
we have
$$
[\hat P_i^2,\ \hat T_1(a)\hat T_2(a)] = 0 \quad \text{for } i = 1,2,
$$
because $[\hat P_i,\hat P_j] = 0 \text{ for all } i,j.$

Related: [[Translational Invariance and Momentum Conservation]], [[Two-Body Hamiltonian]]
