Hamiltonian for two interacting particles with central potential.
## Standard Form
$$Ĥ = \frac{\hat P_1^2}{2m_1} + \frac{\hat P_2^2}{2m_2} + V(|r̂_1 - r̂_2|)$$
where:
- $\hat P_1, \hat P_2$ are momentum operators for particles 1 and 2
- m₁, m₂ are their masses
- $V(|r̂_1 - r̂_2|)$ is potential energy depending only on separation distance
**Key assumption**: Potential depends only on magnitude of separation, not on individual positions or direction.
## Two-Particle Position States
Basis states: $|r_1, r_2⟩ = |r_1⟩ \otimes |r_2⟩$
Generic state: $|ψ⟩ = \int\int d^3r_1d^3r_2 |r_1, r_2⟩⟨r_1, r_2|ψ⟩$
## Individual Translation Operators
Can translate each particle independently:
- $\hat T_1(a)|r_1, r_2⟩ = |r_1 + a, r_2⟩$
- $\hat T_2(a)|r_1, r_2⟩ = |r_1, r_2+a⟩$
These commute: $[\hat T_1(a), \hat T_2(a)] = 0$, so $[\hat P_1, \hat P_2] = 0$
## Total Translation
$$\hat T_1(a)\hat T_2(a) = e^{-i(\hat P_1 + \hat P_2)·a/ℏ} = e^{-i\hat P\cdot a/ℏ}$$
where $\hat P = \hat P_1 + \hat P_2$ is the total momentum operator.
## Translational Invariance
**Key property**: $[\hat H, \hat T_1(a)\hat T_1(a)] = 0$
Translating both particles by the same amount doesn't change the distance between them, so $V(|r̂₁ - r̂₂|)$ remains unchanged.
**Consequence**: $[\hat H, \hat P] = 0$ → total momentum is conserved.

Related: [[Translational Invariance and Momentum Conservation]], [[Separation of Two-Body Hamiltonian]], [[Two-Body Hamiltonian commutes with total momentum]]
