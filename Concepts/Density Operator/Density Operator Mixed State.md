For a mixed state where system is in state |ψₖ⟩ with classical probability pₖ:
$$\hat{\rho} = \sum_k p_k |\psi_k\rangle\langle\psi_k|$$

where:
- pₖ ≥ 0 (probabilities)
- Σₖ pₖ = 1 (normalization)

## Properties
**Hermiticity**: ρ† = ρ
$$\rho_{ij} = \sum_k p_k \langle i|\psi_k\rangle\langle\psi_k|j\rangle = \rho_{ji}^*$$

**Normalization**: tr ρ = 1
$$\text{tr } \hat{\rho} = \sum_k p_k \sum_i \langle i|\psi_k\rangle\langle\psi_k|i\rangle = \sum_k p_k = 1$$

**Non-idempotency**: ρ² ≠ ρ
$$\text{tr } \hat{\rho}^2 = \sum_k p_k^2 < \sum_k p_k = 1$$
Therefore: **tr ρ² < 1** (signature of mixed states)

## Diagonalization
Can always diagonalize ρ (it's Hermitian):
$$\hat{\rho} \rightarrow \begin{pmatrix} p_1 & 0 & 0 \\ 0 & p_2 & 0 \\ 0 & 0 & p_3 \end{pmatrix}$$
Diagonal elements are probabilities pₖ.

Then: tr ρ² = p₁² + p₂² + p₃² < 1 (unless one pₖ = 1)

## Matrix Representation
In basis {|i⟩}:
$$\rho_{ij} = \sum_k p_k \langle i|\psi_k\rangle\langle\psi_k|j\rangle$$

### Example: 50-50 Mix of |±z⟩
$$\hat{\rho} = \frac{1}{2}|+z\rangle\langle+z| + \frac{1}{2}|-z\rangle\langle-z| \rightarrow \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$$

Note: **No off-diagonal elements** → no quantum coherence between states.

### Example: 50% |+z⟩, 50% |-x⟩
$$\hat{\rho} = \frac{1}{2}|+z\rangle\langle+z| + \frac{1}{2}|-x\rangle\langle-x| \rightarrow \frac{1}{2}\begin{pmatrix} 3 & -1 \\ -1 & 1 \end{pmatrix}$$
In Sᵤ basis. Note tr ρ² = 1/2(9/4 + 1/4) = 5/8 < 1.

## Calculating Observables
**Probability of measuring state |ϕ⟩**:
$$P(\phi) = \text{tr}(|\phi\rangle\langle\phi| \hat{\rho})$$

**Expectation value** (average of expectation values):
$$\langle\hat{A}\rangle = \text{tr}(\hat{A}\hat{\rho}) = \sum_k p_k \langle\psi_k|\hat{A}|\psi_k\rangle$$

## Time Evolution
Same as pure states:
$$i\hbar\frac{d\hat{\rho}}{dt} = [\hat{H}, \hat{\rho}]$$

## Physical Interpretation
Mixed state represents classical uncertainty: we don't know which quantum state |ψₖ⟩ the system occupies, only probabilities pₖ.

Different from [[Quantum States and Amplitudes|superposition]]: no quantum interference between the states |ψₖ⟩.

## Key Insight: Non-Uniqueness
**Same density operator can arise from different mixtures!**

Example: ρ = (1/2)I can be prepared as:
- 50% |+z⟩, 50% |-z⟩
- 50% |+x⟩, 50% |-x⟩  
- 50% |+y⟩, 50% |-y⟩
- 50% |+n⟩, 50% |-n⟩ for ANY direction n

All give identical predictions for ALL observables → same quantum state!

## Related
- [[Density Operator Pure State]]
- [[Off-Diagonal Elements and Coherence]]
- [[Trace of Density Operator]]
- [[Expectation Values from Density Operator]]