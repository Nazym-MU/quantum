$$\hat{H} = \frac{2A}{\hbar^2}\hat{S}_1 \cdot \hat{S}_2$$
## Operator Identity
$$2\hat{S}_1 \cdot \hat{S}_2 = \hat{S}_{1+}\hat{S}_{2-} + \hat{S}_{1-}\hat{S}_{2+} + 2\hat{S}_{1z}\hat{S}_{2z}$$
- Diagonal terms: from Ŝ₁zŜ₂z
- Off-diagonal terms: from ladder operators
## Basis States
$$|1\rangle = |+z,+z\rangle, \quad |2\rangle = |+z,-z\rangle$$
$$|3\rangle = |-z,+z\rangle, \quad |4\rangle = |-z,-z\rangle$$
## Diagonal Elements
### Element (1|H|1): Both Spins Up
$$\langle+z,+z|\hat{H}|+z,+z\rangle = \frac{A}{\hbar^2}\langle+z,+z|2\hat{S}_{1z}\hat{S}_{2z}|+z,+z\rangle= \frac{A}{\hbar^2} \cdot 2 \cdot \frac{\hbar}{2} \cdot \frac{\hbar}{2} = \frac{A}{2}$$
Ladder operators give zero (can't raise |+z⟩).
### Element (2|H|2): Antiparallel
$$\langle+z,-z|\hat{H}|+z,-z\rangle = \frac{A}{\hbar^2} \cdot 2 \cdot \frac{\hbar}{2} \cdot \left(-\frac{\hbar}{2}\right) = -\frac{A}{2}$$
## Off-Diagonal Elements

### Element (2|H|3)
$$\langle+z,-z|\hat{H}|-z,+z\rangle = \frac{A}{\hbar^2}\langle+z,-z|\hat{S}_{1-}\hat{S}_{2+}|-z,+z\rangle$$
1. $\hat{S}_{2+}|+z\rangle_2 = \hbar|+z\rangle_2$ (raise spin 2)
2. $\hat{S}_{1-}|-z\rangle_1 = \hbar|+z\rangle_1$ (lower spin 1)
$$\langle+z,-z|\hbar^2|+z,-z\rangle = \hbar^2$$
Matrix element: $\frac{A}{\hbar^2} \cdot \hbar^2 = A$
### Element (3|H|2): Hermiticity
By Hermiticity of Ĥ:
$$(3|H|2) = (2|H|3)^* = A$$
Final Matrix in basis {|+z,+z⟩, |+z,-z⟩, |-z,+z⟩, |-z,-z⟩}:
$$\hat{H} = \begin{pmatrix} 
A/2 & 0 & 0 & 0 \\ 
0 & -A/2 & A & 0 \\ 
0 & A & -A/2 & 0 \\ 
0 & 0 & 0 & A/2 
\end{pmatrix}$$
## Diagonalization
Middle 2×2 block has eigenvalues:
$$E_{\pm} = -\frac{A}{2} \pm A = \begin{cases} +A/2 & \text{(symmetric)} \\ -3A/2 & \text{(antisymmetric)} \end{cases}$$
**Eigenstates**:
- Triplet (E = A/2): |+z,+z⟩, symmetric superposition, |-z,-z⟩
- Singlet (E = -3A/2): antisymmetric superposition
## Related
- [[Hyperfine Splitting]]
- [[Raising and Lowering Operators]]
- [[Spin-Spin Interaction]]