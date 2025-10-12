## Orthonormal Basis
### Definition
A set of states ${|a_i\rangle}$ forms an orthonormal basis if:
$$\langle a_i|a_j\rangle = \delta_{ij} = \begin{cases} 1 & i = j \\ 0 & i \neq j \end{cases}$$

- **Orthogonal**: Different basis states have zero overlap
- **Normal**: Each basis state is normalized to 1
### Examples
**$S_z$ basis**: {|+z⟩, |-z⟩}
- ⟨+z|+z⟩ = 1, ⟨-z|-z⟩ = 1
- ⟨+z|-z⟩ = 0

**$S_x$ basis**: {|+x⟩, |-x⟩}
- Also orthonormal but different from $S_z$ basis
## Completeness Relation

A complete basis satisfies:
$$\sum_i |a_i\rangle\langle a_i| = \hat{I}$$

Î - [[Identity Operators]].
### For Spin-1/2
$$|+z\rangle\langle+z| + |-z\rangle\langle-z| = \hat{I}$$
Also written using [[Projection Operators]]
$$\hat{P}_+ + \hat{P}_- = \hat{I}$$
## Expanding Arbitrary States
Any state |ψ⟩ can be written in terms of a complete basis:
$$|\psi\rangle = \hat{I}|\psi\rangle = \sum_i |a_i\rangle\langle a_i|\psi\rangle = \sum_i c_i|a_i\rangle$$
where cᵢ = ⟨aᵢ|ψ⟩ are the components/amplitudes.
## Multiple Bases
The same state can be expressed in different bases:
**$S_z$ basis**:
$$|\psi\rangle = c_+|+z\rangle + c_-|-z\rangle$$
**$S_x$ basis**:
$$|\psi\rangle = d_+|+x\rangle + d_-|-x\rangle$$
These are different representations of the same physical state.
## Related
- [[Basis Transformations]]
- [[Quantum States and Amplitudes]]