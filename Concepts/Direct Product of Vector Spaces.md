## Definition

A way to combine two vector spaces to form a larger product space. For quantum systems, this describes composite systems made of multiple particles.
$$|\psi\rangle_1 \otimes |\phi\rangle_2$$
Often simplified to:
- $|\psi\rangle_1|\phi\rangle_2$
- $|\psi, \phi\rangle$
The symbol ⊗ (tensor product) emphasizes we're combining vectors from **different** vector spaces.
### Dimension
If space 1 has dimension $d_1$ and space 2 has dimension $d_2$: $$\text{dim}(\mathcal{H}_1 \otimes \mathcal{H}_2) = d_1 \times d_2$$
Basis states from different spaces are linearly independent, even if they use the same symbols:
- $|+z\rangle_1$ and $|+z\rangle_2$ are **different** vectors
- They live in different vector spaces
- $|+z, +z\rangle$ is perfectly valid and independent
### Inner Products

$$\langle \psi_1, \phi_1 | \psi_2, \phi_2 \rangle = \langle \psi_1 | \psi_2 \rangle \cdot \langle \phi_1 | \phi_2 \rangle$$
The inner product factors into products of inner products in each space.
## Operators on Product Spaces

### Single-Particle Operators

An operator acting only on particle 1: $\hat{A}_1 \otimes \hat{I}_2$ acts on particle 1, leaves particle 2 unchanged.
### Commutation Relations

Operators on different particles always commute: $$[\hat{A}_1, \hat{B}_2] = 0$$
## Contrast with Other Products

**Inner product:** $\langle \phi | \psi \rangle$ → scalar

- Vectors from the **same** space

**Outer product:** $|\psi\rangle\langle\phi|$ → operator

- Vectors from the **same** space

**Direct product:** $|\psi\rangle_1 \otimes |\phi\rangle_2$ → vector in larger space

- Vectors from **different** spaces

## Related Concepts

- [[Two-Particle Spin Systems]]
- [[Inner product]]
- [[Quantum State Vector]]
- [[Matrix Mechanics]]