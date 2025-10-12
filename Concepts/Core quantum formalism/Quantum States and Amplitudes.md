## Quantum State as Superposition
A general quantum state can be written as a linear combination of basis states:
$$|\psi⟩ = \sum_n c_n |a_n⟩$$
where:
- $|a_n\rangle$ are orthonormal basis states
- $c_n$ are complex coefficients (probability amplitudes)
## Probability Amplitudes
### Definition
The amplitude cₙ = ⟨aₙ|ψ⟩ is a complex number whose absolute square gives the probability:
$$P(a_n) = |c_n|^2 = |\langle a_n|\psi\rangle|^2$$
### Properties
- Complex valued: $c_n = |c_n|e^{(iδ_n)}$
- Magnitude: |$c_n$| determines probability
- Phase: $δ_n$ determines interference effects
- Not directly observable (only $|c_n|^2$ is)
## Normalization Condition
Probabilities must sum to 1:
$$\langle\psi|\psi\rangle = \sum_n |c_n|^2 = 1$$
Derivation using basis orthonormality [[(4)]]:
$$\langle\psi|\psi\rangle = \langle\psi|+z\rangle\langle+z|\psi\rangle + \langle\psi|-z\rangle\langle-z|\psi\rangle = |c_+|^2 + |c_-|^2 = 1$$
## Example: Spin-1/2 States
For $|+x\rangle$ state in $S_z$ basis:
$$|+x\rangle = \frac{1}{\sqrt{2}}|+z\rangle + \frac{1}{\sqrt{2}}|-z\rangle$$
- c₊ = 1/√2, so P(S_z = +ℏ/2) = |1/√2|² = 1/2
- c₋ = 1/√2, so P(S_z = -ℏ/2) = |1/√2|² = 1/2
Equal probability of measuring either outcome.
## Physical Interpretation
**Amplitude**: Encodes both probability (via magnitude) and phase relationships
**State Vector**: Complete description of quantum system at a given time
**Measurement**: Collapses superposition to one basis state with probability |cₙ|²
## Related
- [[Bra-Ket Notation]]
- [[Expectation value]]
- [[Relative phases]]
- [[Stern-Gerlach Experiments]]