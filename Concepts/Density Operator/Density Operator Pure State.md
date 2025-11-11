For a pure state |ψ⟩, the density operator is:
$$\hat{\rho} = |\psi\rangle\langle\psi|$$

## Properties
**Hermiticity**: ρ† = ρ
- Matrix elements: ρᵢⱼ = ⟨i|ψ⟩⟨ψ|j⟩ = ⟨ψ|j⟩*⟨i|ψ⟩* = ρⱼᵢ*

**Normalization**: tr ρ = 1
$$\text{tr } \hat{\rho} = \sum_i \langle i|\psi\rangle\langle\psi|i\rangle = \langle\psi|\psi\rangle = 1$$

**Idempotency**: ρ² = ρ
$$\hat{\rho}^2 = |\psi\rangle\langle\psi|\psi\rangle\langle\psi| = |\psi\rangle\langle\psi| = \hat{\rho}$$
Therefore: **tr ρ² = 1** (signature of pure states)

## Connection to Projection Operators
The density operator for a pure state IS the [[Projection Operators|projection operator]] for that state:
$$\hat{P}_\psi = |\psi\rangle\langle\psi|$$

## Matrix Representation
In basis {|i⟩}:
$$\rho_{ij} = \langle i|\psi\rangle\langle\psi|j\rangle$$

### Examples
**State |+z⟩ in Sᵤ basis**:
$$\hat{\rho} = |+z\rangle\langle+z| \rightarrow \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$$

**State |+y⟩ = (1/√2)(|+z⟩ + i|-z⟩) in Sᵤ basis**:
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$
Note: Off-diagonal elements encode the relative phase between |+z⟩ and |-z⟩.

## Calculating Observables
**Probability of measuring state |ϕ⟩**:
$$P(\phi) = \text{tr}(|\phi\rangle\langle\phi| \hat{\rho}) = |\langle\phi|\psi\rangle|^2$$

**Expectation value of observable Â**:
$$\langle\hat{A}\rangle = \text{tr}(\hat{A}\hat{\rho}) = \langle\psi|\hat{A}|\psi\rangle$$

## Time Evolution
From Schrödinger equation iℏ∂|ψ⟩/∂t = Ĥ|ψ⟩:
$$i\hbar\frac{d\hat{\rho}}{dt} = [\hat{H}, \hat{\rho}]$$

## Physical Interpretation
Pure state represents maximal knowledge: system is definitely in state |ψ⟩. No classical uncertainty about which quantum state the system occupies.

## Related
- [[Density Operator Mixed State]] (generalization)
- [[Projection Operators]]
- [[Expectation Values]]
- [[Quantum States and Amplitudes]]