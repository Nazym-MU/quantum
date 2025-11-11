For observable Â with density operator ρ:
$$\langle\hat{A}\rangle = \text{tr}(\hat{A}\hat{\rho})$$

This formula works for both pure and mixed states.

## Derivation for Pure States
For ρ = |ψ⟩⟨ψ|:
$$\langle\hat{A}\rangle = \text{tr}(\hat{A}|\psi\rangle\langle\psi|) = \sum_i \langle i|\hat{A}|\psi\rangle\langle\psi|i\rangle$$
$$= \sum_i \langle\psi|i\rangle\langle i|\hat{A}|\psi\rangle = \langle\psi|\hat{A}|\psi\rangle$$
Using completeness: Σᵢ |i⟩⟨i| = I

## Derivation for Mixed States
For ρ = Σₖ pₖ|ψₖ⟩⟨ψₖ|:
$$\langle\hat{A}\rangle = \text{tr}(\hat{A}\hat{\rho}) = \sum_k p_k \text{tr}(\hat{A}|\psi_k\rangle\langle\psi_k|)$$
$$= \sum_k p_k \langle\psi_k|\hat{A}|\psi_k\rangle$$

This is the **probability-weighted average** of expectation values for each pure state.

## Matrix Form
In basis {|i⟩}:
$$\langle\hat{A}\rangle = \sum_{i,j} \langle i|\hat{A}|j\rangle \langle j|\hat{\rho}|i\rangle = \sum_{i,j} A_{ij} \rho_{ji}$$

**Note the indices**: Aᵢⱼρⱼᵢ (not Aᵢⱼρᵢⱼ)

This comes from the trace definition: tr(ÂB̂) = Σᵢ⟨i|ÂB̂|i⟩ sums over diagonal elements of the product.

## Step-by-Step Calculation
1. Write Â in chosen basis (e.g., Sᵤ basis for spin operators)
2. Write ρ in same basis
3. Compute matrix product Âρ
4. Sum diagonal elements: ⟨Â⟩ = Σᵢ(Âρ)ᵢᵢ

### Example: ⟨Sᵧ⟩ for |+z⟩
$$\hat{S}_y = \frac{\hbar}{2}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}, \quad \hat{\rho} = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$$

$$\hat{S}_y\hat{\rho} = \frac{\hbar}{2}\begin{pmatrix} 0 & 0 \\ i & 0 \end{pmatrix}$$

$$\langle S_y\rangle = \text{tr}(\hat{S}_y\hat{\rho}) = \frac{\hbar}{2}(0 + 0) = 0$$

### Example: ⟨Sᵧ⟩ for |+y⟩
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$

$$\hat{S}_y\hat{\rho} = \frac{\hbar}{2}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} \frac{1}{2}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix} = \frac{\hbar}{4}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$

$$\langle S_y\rangle = \text{tr}(\hat{S}_y\hat{\rho}) = \frac{\hbar}{4}(1 + 1) = \frac{\hbar}{2}$$

As expected! |+y⟩ is eigenstate of Ŝᵧ with eigenvalue ℏ/2.

## Using Identity Operator
The calculation uses completeness at multiple steps:
$$\langle\hat{A}\rangle = \text{tr}(\hat{A}\hat{\rho}) = \sum_i \langle i|\hat{A}\hat{\rho}|i\rangle$$
$$= \sum_{i,j} \langle i|\hat{A}|j\rangle\langle j|\hat{\rho}|i\rangle$$

The insertion of Σⱼ |j⟩⟨j| = I between  and ρ̂ allows us to write in matrix form.

## Related
- [[Expectation Values]] (standard formalism)
- [[Trace of Density Operator]]
- [[Density Operator Pure State]]
- [[Density Operator Mixed State]]
- [[Matrix Representations]]