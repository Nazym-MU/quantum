## Definitions
- $\hat{J}$ - vector operator composed of three operators: $\hat{J}_x$, $\hat{J}_y$, $\hat{J}_z$ - Hermitian operators corresponding to angular momentum projections on the x, y, z axes
- $\hat{J^2}$ - squared magnitude of the total angular momentum: $\hat{J}^2 = \hat{J}_x^2 + \hat{J}_y^2 + \hat{J}_z^2$
## Properties
### Non-negativity of Eigenvalues
- Since $\hat{J}^2$ is built from sums of squared Hermitian operators, its eigenvalues must be $\geq 0$
- $⟨ψ∣J^2∣ψ⟩≥0$: For any operator $A^\dagger A$, the expectation value is non-negative [[(12)]]
### Commutation Relations
- $J^2$ commutes with each projection [[(10)]]: $[\hat{J}^2, \hat{J}_z] = 0$ (similarly for $x$ and $y$)
- Therefore, they have simultaneous eigenstates in common [[(11)]]:
    - $\hat{J^2}\ket{\lambda, m} = \lambda \hbar^2\ket{\lambda, m}$
    - $\hat{J}_z\ket{\lambda, m}=m\hbar \ket{\lambda, m}$
- However, the components don't commute with each other:
    - $[\hat{J}_x, \hat{J}_y] = i\hbar\hat{J}_z$
    - $[\hat{J}_y, \hat{J}_z] = i\hbar\hat{J}_x$
    - $[\hat{J}_z, \hat{J}_x] = i\hbar\hat{J}_y$
### Standard Notation
Conventionally, we relabel $\lambda = j(j+1)$ where $j$ can be integer or half-integer:
- $\hat{J}^2\ket{j, m} = j(j+1)\hbar^2\ket{j, m}$
- $\hat{J}_z\ket{j, m} = m\hbar\ket{j, m}$
### Magnitude of Angular Momentum
$$|\hat{J}| = \hbar\sqrt{j(j+1)}$$
This comes from the eigenvalue of $\hat{J}^2$.
### Range of $m$ values
For a given $j$: $$m \in {-j, -j+1, \ldots, j-1, j}$$
Total number of states: $2j + 1$
## Single-Particle vs. Two-Particle Systems
### Single Particle
- For spin-1/2: $j = 1/2$, $m \in {-1/2, +1/2}$ → 2 states
- Eigenstates: $\ket{+z}$, $\ket{-z}$ (basis for 2D Hilbert space)
### Two Particles
- Each particle has its own angular momentum operators: $\hat{S}_1$ and $\hat{S}_2$
- These operators commute: $[\hat{S}_{1i}, \hat{S}_{2j}] = 0$
- Can form basis states as direct products: $\ket{s_1, s_2}$ (4D space for two spin-1/2)
- Can also use **total angular momentum** basis (see [[Total Angular Momentum]])
### Total Angular Momentum
For two-particle systems, define: $$\hat{S}_{\text{total}} = \hat{S}_1 + \hat{S}_2$$
This is also an angular momentum operator with its own eigenvalue structure.
**Example: Two spin-1/2 particles**
- Can combine to give total spin $S = 0$ (singlet) or $S = 1$ (triplet)
- Singlet: 1 state with $S = 0$, $m_S = 0$
- Triplet: 3 states with $S = 1$, $m_S \in {-1, 0, +1}$
## Connection to Physical Systems
### Hydrogen Hyperfine Structure
The [[Hyperfine Splitting]] eigenstates are eigenstates of both:
- The Hamiltonian $\hat{H} = \frac{A}{\hbar^2}\hat{S}_1 \cdot \hat{S}_2$
- Total spin $\hat{S}^2_{\text{total}}$
Because $[\hat{H}, \hat{S}^2_{\text{total}}] = 0$, we can label states by total spin quantum number.
### Stern-Gerlach Experiments
Sequential measurements demonstrate:
- $\hat{J}_z$ and $\hat{J}_x$ don't commute → can't measure simultaneously
- Measuring one destroys information about the other
- Consistent with uncertainty relations
## Tags
- [[Raising and Lowering Operators]]
- [[Intrinsic spin angular momentum operators]]
- [[Intrinsic spin angular momentum]]
- [[Two-Particle Spin Systems]]
- [[Commutators]]
- [[Hyperfine Splitting]]