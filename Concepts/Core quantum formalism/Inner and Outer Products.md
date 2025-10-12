## Inner Product ⟨φ|ψ⟩
bra + ket → scalar (complex number): $\langle\phi|\psi\rangle = \text{complex number}$
#### Properties
- ⟨φ|ψ⟩ = ⟨ψ|φ⟩* (conjugate symmetry)
- ⟨ψ|ψ⟩ ≥ 0 (positive definite)
- ⟨ψ|ψ⟩ = 1 (normalized states)
#### Physical Meaning
Probability amplitude for state |ψ⟩ to be found in state |φ⟩.
$$P(\phi \text{ in } \psi) = |\langle\phi|\psi\rangle|^2$$
#### For Direct Products
$$\langle\psi_1,\phi_1|\psi_2,\phi_2\rangle = \langle\psi_1|\psi_2\rangle \cdot \langle\phi_1|\phi_2\rangle$$
## Outer Product |ψ⟩⟨φ|
ket + bra → operator: $|\psi\rangle\langle\phi| = \text{operator}$
### Action on States
$$(|\psi\rangle\langle\phi|)|\chi\rangle = |\psi\rangle\langle\phi|\chi\rangle = \langle\phi|\chi\rangle|\psi\rangle$$
Projects |χ⟩ onto |φ⟩, then rescales by result and points along |ψ⟩.
### Matrix Representation
In basis {|1⟩, |2⟩}:
$$|\psi\rangle\langle\phi| \rightarrow \begin{pmatrix} \psi_1\phi_1^* & \psi_1\phi_2^* \\ \psi_2\phi_1^* & \psi_2\phi_2^* \end{pmatrix}$$
Rank-1 matrix (all rows proportional).
## Related
- [[Bra-Ket Notation]]