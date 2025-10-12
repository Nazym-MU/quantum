$$\hat{A}|\psi\rangle = |\phi\rangle$$
## Linear Operators
$$\hat{A}(c_1|\psi_1\rangle + c_2|\psi_2\rangle) = c_1\hat{A}|\psi_1\rangle + c_2\hat{A}|\psi_2\rangle$$
**All quantum mechanical operators are linear:**
1. $Â(c|ψ⟩) = cÂ|ψ⟩$ (scalar multiplication)
2. $Â(|ψ₁⟩ + |ψ₂⟩) = Â|ψ₁⟩ + Â|ψ₂⟩$ (additivity)
## Eigenvalue Equation
$$\hat{A}|\psi\rangle = \lambda|\psi\rangle$$
- $|ψ⟩$ is an **eigenstate** (or eigenvector, eigenket)
- $\lambda$ is the corresponding **eigenvalue** (a number)
**Physical meaning**: Measuring observable Â on eigenstate |ψ⟩ gives definite result a with certainty.
### Example: $J_z$
$$\hat{J}_z|+z\rangle = \frac{\hbar}{2}|+z\rangle$$
Measuring $S_z$ on |+z⟩ gives $+\frac{\hbar}{2}$ with probability 1.
## Types of Operators
### By Mathematical Properties
- **[[Hermitian Operators]]**: Â† = Â (observables)
- **[[Unitary Operators]]**: Û†Û = I (symmetry transformations)
- **[[Projection Operators]]**: $\hat{P}^2=\hat{P}$ (measurement)
### By Physical Role
- **[[Rotation Operators]]**: $\hat{R}$ (spatial/spin rotations)
- **[[Hamiltonian Operator]]**: Ĥ (energy, time evolution)
- **[[Time Evolution Operator]]**: Û(t) (propagates states)
## Action on Bras
Operators act on kets from the left:
$$\hat{A}|\psi\rangle$$
The adjoint operator acts on bras from the right:
$$\langle\psi|\hat{A}^\dagger$$
## Matrix Representation
In a chosen basis {|aᵢ⟩}, operator Â becomes a matrix:
$$A_{ij} = \langle a_i|\hat{A}|a_j\rangle$$
## Operator Algebra
- **Addition**: $(\hat{A} + \hat{B})|ψ⟩ = \hat{A}|ψ⟩ + \hat{B}|ψ⟩$
- **Multiplication**: $(ÂB̂)|ψ⟩ = Â(B̂|ψ⟩)$
- **[[Commutators]]**: $[\hat{A},\hat{B}] = \hat{A}\hat{B}-\hat{B}\hat{A}$
## Physical Interpretation
- Eigenvalues → possible measurement outcomes
- Eigenstates → states with definite values
- Expectation values → probability-weighted average of measurements
## Related
- [[Hermitian Operators]]
- [[Unitary Operators]]
- [[Adjoint Operators]]
- [[Commutators]]
- [[Matrix Mechanics]]