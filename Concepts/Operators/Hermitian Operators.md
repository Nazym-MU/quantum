An operator Â is **Hermitian** (or **self-adjoint**) if:
$$\hat{A}^\dagger = \hat{A}$$
## Key Properties
1. Real eigenvalues: Observable quantities must be real, so observables are represented by Hermitian operators.
$$\hat{A}|\psi\rangle = a|\psi\rangle \implies a \in \mathbb{R}$$
2. Eigenvectors with different eigenvalues are orthogonal:
$$\hat{A}|\psi_1\rangle = a_1|\psi_1\rangle, \quad \hat{A}|\psi_2\rangle = a_2|\psi_2\rangle, \quad a_1 \neq a_2 \implies \langle\psi_1|\psi_2\rangle = 0$$
3. Eigenvectors form a complete orthonormal basis (for finite-dimensional spaces).
## Matrix Representation
A matrix $M$ is Hermitian if:
$$M^\dagger = M^T* = M$$
Equivalent conditions:
- M†= M (conjugate transpose equals original)
### Example: $J_z$ Matrix
$$\hat{J}_z \xrightarrow[S_z\text{ basis}]{} \frac{\hbar}{2}\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$$
## Physical Observables
All quantum mechanical observables correspond to Hermitian operators:
- Position: $\hat{x}$
- Momentum:  $\hat{p}$
- Angular momentum:  $\hat{J}$,  $\hat{S}$,  $\hat{J}$
- Energy:  $\hat{H}$ (Hamiltonian)
- Spin components:  $\hat{S_x}$, $\hat{S_y}$, $\hat{S_z}$
## Derivations:
- [[Hermiticity of J_z]]
- [[Why Real Eigenvalues in Hermitian]]
## Related
- [[Unitary Operators]]
- [[Adjoint Operators]]
- [[Hamiltonian Operator]]