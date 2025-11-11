# Trace of Density Operator

The trace sums diagonal matrix elements of an operator in any basis:
$$\text{tr } \hat{\rho} = \sum_i \langle i|\hat{\rho}|i\rangle$$

## Key Property: Basis Independence
The trace gives the same value in ANY basis {|i⟩}. This makes it useful for calculating physical observables.

## For Pure States
$$\hat{\rho} = |\psi\rangle\langle\psi|$$
$$\text{tr } \hat{\rho} = \sum_i \langle i|\psi\rangle\langle\psi|i\rangle = \langle\psi|\psi\rangle = 1$$

Using completeness relation: Σᵢ |i⟩⟨i| = I

## For Mixed States
$$\hat{\rho} = \sum_k p_k |\psi_k\rangle\langle\psi_k|$$
$$\text{tr } \hat{\rho} = \sum_k p_k \sum_i \langle i|\psi_k\rangle\langle\psi_k|i\rangle = \sum_k p_k = 1$$

## Cyclic Property
$$\text{tr}(\hat{A}\hat{B}) = \text{tr}(\hat{B}\hat{A})$$

Proof in discrete basis:
$$\text{tr}(\hat{A}\hat{B}) = \sum_i \langle i|\hat{A}\hat{B}|i\rangle = \sum_{i,j} \langle i|\hat{A}|j\rangle\langle j|\hat{B}|i\rangle$$
$$= \sum_{j,i} \langle j|\hat{B}|i\rangle\langle i|\hat{A}|j\rangle = \sum_j \langle j|\hat{B}\hat{A}|j\rangle = \text{tr}(\hat{B}\hat{A})$$

This allows swapping order in expectation value calculations.

## Trace of ρ²: Purity Test
**Pure state**: ρ² = ρ, so:
$$\text{tr } \hat{\rho}^2 = \text{tr } \hat{\rho} = 1$$

**Mixed state**: ρ in diagonal form has ρ = diag(p₁, p₂, ...), so:
$$\text{tr } \hat{\rho}^2 = \sum_k p_k^2 < \left(\sum_k p_k\right)^2 = 1$$

Since pₖ < 1 for all k (probabilities), each pₖ² < pₖ.

**Test**: tr ρ² = 1 ⟺ pure state; tr ρ² < 1 ⟺ mixed state

## Calculating Probabilities
Probability of measuring state |ϕ⟩:
$$P(\phi) = \text{tr}(|\phi\rangle\langle\phi| \hat{\rho}) = \text{tr}(\hat{P}_\phi \hat{\rho})$$

For pure state ρ = |ψ⟩⟨ψ|:
$$P(\phi) = \text{tr}(|\phi\rangle\langle\phi|\psi\rangle\langle\psi|) = \langle\phi|\psi\rangle\langle\psi|\phi\rangle = |\langle\phi|\psi\rangle|^2$$

## Why "Trace"?
Historical: "Trace" comes from German "Spur" (track/trace). It refers to "tracing" along the diagonal of a matrix. Used in mathematics since 1800s.

## Related
- [[Expectation Values from Density Operator]]
- [[Density Operator Pure State]]
- [[Density Operator Mixed State]]
- [[Matrix Representations]]