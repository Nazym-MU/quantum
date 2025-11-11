For pure states, the density operator IS a projection operator.
## Projection Operator Definition
Projection operator onto state |ψ⟩:
$$\hat{P}_\psi = |\psi\rangle\langle\psi|$$
Properties:
- Hermitian: P̂†ₚₛᵢ = P̂ₚₛᵢ
- Idempotent: P̂²ₚₛᵢ = P̂ₚₛᵢ
- Projects any state onto |ψ⟩: P̂ₚₛᵢ|ϕ⟩ = ⟨ψ|ϕ⟩|ψ⟩

## Pure State Density Operator
$$\hat{\rho} = |\psi\rangle\langle\psi|$$

This is EXACTLY the projection operator for |ψ⟩!

## Shared Properties
Both P̂ₚₛᵢ and ρ̂ (for pure states) satisfy:

**Hermiticity**:
$$\hat{\rho}^\dagger = (|\psi\rangle\langle\psi|)^\dagger = |\psi\rangle\langle\psi| = \hat{\rho}$$

**Idempotency**:
$$\hat{\rho}^2 = |\psi\rangle\langle\psi|\psi\rangle\langle\psi| = |\psi\rangle\langle\psi| = \hat{\rho}$$

**Normalization**:
$$\text{tr}(\hat{\rho}) = \langle\psi|\psi\rangle = 1$$

**Unit trace of square**:
$$\text{tr}(\hat{\rho}^2) = \text{tr}(\hat{\rho}) = 1$$

## Physical Interpretation
The density operator for pure state |ψ⟩:
- Projects measurements onto the |ψ⟩ component
- Encodes complete information about the pure state
- Gives probability |⟨ϕ|ψ⟩|² for measuring |ϕ⟩

## Probability Calculation
Probability of measuring state |ϕ⟩ when system is in pure state ρ̂ = |ψ⟩⟨ψ|:

$$P(\phi) = \text{tr}(|\phi\rangle\langle\phi| \hat{\rho})$$
$$= \text{tr}(|\phi\rangle\langle\phi|\psi\rangle\langle\psi|)$$
$$= \langle\phi|\psi\rangle\langle\psi|\phi\rangle = |\langle\phi|\psi\rangle|^2$$

This uses the projection operator |ϕ⟩⟨ϕ| to extract the probability.

## Mixed States: NOT Projection Operators
For mixed states ρ̂ = Σₖ pₖ|ψₖ⟩⟨ψₖ|:

$$\hat{\rho}^2 = \sum_{k,k'} p_k p_{k'} |\psi_k\rangle\langle\psi_k|\psi_{k'}\rangle\langle\psi_{k'}|$$

For orthogonal states ⟨ψₖ|ψₖ'⟩ = δₖₖ':
$$\hat{\rho}^2 = \sum_k p_k^2 |\psi_k\rangle\langle\psi_k| \neq \hat{\rho}$$

**Not idempotent** → not a projection operator!
## Conceptual Link
Pure state density operator as projection operator shows:
- Quantum state is determined by projection onto basis states
- Measuring = projecting onto measurement basis
- Density operator framework unifies state description with measurement
## Related
- [[Projection Operators]]
- [[Density Operator Pure State]]
- [[Density Operator Mixed State]]
- [[Measurement and State Collapse]]