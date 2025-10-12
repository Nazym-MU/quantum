## From General to Spin-1/2
Relabeling from general angular momentum Ĵ to intrinsic spin Ŝ for s = 1/2:
**Eigenvalue equations**:
$$\hat{S}^2|s,m\rangle = s(s+1)\hbar^2|s,m\rangle = \frac{3}{4}\hbar^2|s,m\rangle$$
$$\hat{S}_z|s,m\rangle = m\hbar|s,m\rangle$$

where m = $±1/2$ for spin-1/2.
## Pauli Spin Matrices
The spin operators in the $S_z$ basis {|+z⟩, |-z⟩}:

$$\hat{S}_z = \frac{\hbar}{2}\sigma_z = \frac{\hbar}{2}\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} \qquad \hat{S}_x = \frac{\hbar}{2}\sigma_x = \frac{\hbar}{2}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \qquad \hat{S}_y = \frac{\hbar}{2}\sigma_y = \frac{\hbar}{2}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}$$
where $σ_x, σ_y, σ_z$ are the dimensionless **Pauli matrices**.
## Properties of Pauli Matrices
- [[Hermitian Operators|Hermitian]], so they represent observables.
- Each has eigenvalues **±1**. This gives S_i eigenvalues of ±ℏ/2 (after multiplying by ℏ/2).
- Trace: $\text{Tr}(\sigma_i) = 0$. Sum of eigenvalues is zero (one positive, one negative).
- $\det(\sigma_i) = -1$
- Anticommutation: $\{\sigma_i, \sigma_j\} = \sigma_i\sigma_j + \sigma_j\sigma_i = 2\delta_{ij}I$
	- When $i ≠ j$: they anticommute (sum = 0)
	- When $i = j$: $σ^2_i = I$
- Products: $\sigma_x\sigma_y = i\sigma_z \qquad \sigma_y\sigma_z = i\sigma_x \qquad \sigma_z\sigma_x = i\sigma_y$
- Squares: $\sigma_x^2 = \sigma_y^2 = \sigma_z^2 = I$
- Commutation Relations in terms of Pauli matrices: $[\sigma_i, \sigma_j] = 2i\epsilon_{ijk}\sigma_k$
- Eigenstates:
	- $S_z$ eigenstates (diagonal): $\hat{S}_z|\pm z\rangle = \pm\frac{\hbar}{2}|\pm z\rangle, \quad |+z\rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix}\quad |-z\rangle = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$
	- $S_x$ eigenstates: $|+x\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ 1 \end{pmatrix}, \quad |-x\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ -1 \end{pmatrix}$
	- $S_y$ eigenstates: $|+y\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ i \end{pmatrix}, \quad |-y\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ -i \end{pmatrix}$
### Spin along arbitrary direction for unit vector $\hat{n} = (n_x, n_y, n_z)$:
$$\hat{S}_{\hat{n}} = \vec{S} \cdot \hat{n} = \frac{\hbar}{2}(\vec{\sigma} \cdot \hat{n})$$
$$\hat{S}_{\hat{n}} = \frac{\hbar}{2}\begin{pmatrix} n_z & n_x - in_y \\ n_x + in_y & -n_z \end{pmatrix}$$
This has eigenvalues ±ℏ/2 for **any** direction $\hat{n}$.
## Related
- [[Spin-1-2 Systems]]
- [[Eigenvalue Structure]]
- [[Raising and Lowering Operators]]