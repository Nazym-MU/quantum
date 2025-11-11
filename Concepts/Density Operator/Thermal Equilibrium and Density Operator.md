Density operator framework for systems in thermal equilibrium at temperature T.
## Boltzmann Distribution
For system with Hamiltonian Ĥ, thermal equilibrium density operator:
$$\hat{\rho} = \frac{1}{Z} e^{-\hat{H}/k_B T}$$

where:
- kᴮ = Boltzmann constant
- T = temperature
- Z = partition function (normalization)

## Partition Function
$$Z = \text{tr}(e^{-\hat{H}/k_B T}) = \sum_n e^{-E_n/k_B T}$$

Ensures tr ρ = 1 (probability normalization).

## For Spin-½ in Magnetic Field
Hamiltonian: Ĥ = -μB̂ₖ·Ŝᵤ = -μBŜᵤ

Energy eigenvalues:
- E₊ = -μB (for |+z⟩)
- E₋ = +μB (for |-z⟩)

where μ = geℏ/(4mₑc) ≈ μᴮ (Bohr magneton for electron).

## Density Operator
$$\hat{\rho} = \frac{1}{Z}\left(e^{\mu B/k_B T}|+z\rangle\langle+z| + e^{-\mu B/k_B T}|-z\rangle\langle-z|\right)$$

Partition function:
$$Z = e^{\mu B/k_B T} + e^{-\mu B/k_B T} = 2\cosh(\mu B/k_B T)$$

Matrix representation in Sᵤ basis:
$$\hat{\rho} = \frac{1}{Z}\begin{pmatrix} e^{\mu B/k_B T} & 0 \\ 0 & e^{-\mu B/k_B T} \end{pmatrix}$$

## Magnetization
Average magnetic moment for N particles:
$$M = N\langle\mu_z\rangle = N \cdot \text{tr}(\mu \hat{S}_z \hat{\rho})$$

Calculation:
$$M = N\mu \frac{e^{\mu B/k_B T} - e^{-\mu B/k_B T}}{e^{\mu B/k_B T} + e^{-\mu B/k_B T}} = N\mu \tanh(\mu B/k_B T)$$

## Curie's Law (High Temperature Limit)
When μB/kᴮT ≪ 1:
$$\tanh(x) \approx x \text{ for } x \ll 1$$

Therefore:
$$M \approx N\mu \frac{\mu B}{k_B T} = \frac{N\mu^2 B}{k_B T} = \frac{C B}{T}$$

where C = Nμ²/kᴮ is the **Curie constant**.

This 1/T dependence is **Curie's law** for paramagnetism (discovered experimentally by Pierre Curie).

## Physical Interpretation
At high temperature (kᴮT ≫ μB):
- Thermal energy dominates → states nearly equally populated
- ρ ≈ (1/2)I (unpolarized)
- Weak magnetization

At low temperature (kᴮT ≪ μB):
- Energy differences dominate → mostly in ground state |+z⟩
- Strong magnetization M → Nμ

## Key Properties
- Mixed state (thermal mixture, not superposition)
- No off-diagonal elements in energy basis
- tr ρ² < 1 (not a pure state)
- Time-independent if Ĥ time-independent

## Related
- [[Density Operator Mixed State]]
- [[Hamiltonian Operator]]
- [[Stationary States]]
- [[Magnetic Moment]]