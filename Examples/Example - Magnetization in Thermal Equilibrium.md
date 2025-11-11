# Example - Magnetization in Thermal Equilibrium

Calculating magnetization of spin-½ particles in thermal equilibrium using density operator.

## Setup
- N spin-½ particles
- Magnetic field B = B**k** (z-direction)
- Temperature T
- Hamiltonian: Ĥ = -(geℏ/4mₑc)B·Ŝ = -μBŜᵤ
- Magnetic moment: μ = geℏ/(4mₑc) ≈ μᴮ (Bohr magneton)

## Energy Eigenvalues
$$\hat{H}|+z\rangle = -\mu B|+z\rangle \quad (E_+ = -\mu B)$$
$$\hat{H}|-z\rangle = +\mu B|-z\rangle \quad (E_- = +\mu B)$$

Lower energy state: |+z⟩ (aligned with field)

## Thermal Density Operator
In thermal equilibrium at temperature T:
$$\hat{\rho} = \frac{1}{Z}e^{-\hat{H}/k_B T}$$

where Z = partition function (normalization).

**Explicit form**:
$$\hat{\rho} = \frac{1}{Z}\left(e^{-E_+/k_B T}|+z\rangle\langle+z| + e^{-E_-/k_B T}|-z\rangle\langle-z|\right)$$

$$= \frac{1}{Z}\left(e^{\mu B/k_B T}|+z\rangle\langle+z| + e^{-\mu B/k_B T}|-z\rangle\langle-z|\right)$$

## Partition Function
$$Z = \text{tr}(e^{-\hat{H}/k_B T}) = e^{\mu B/k_B T} + e^{-\mu B/k_B T}$$

$$Z = 2\cosh(\mu B/k_B T)$$

## Matrix in Sᵤ Basis
$$\hat{\rho} = \frac{1}{Z}\begin{pmatrix} e^{\mu B/k_B T} & 0 \\ 0 & e^{-\mu B/k_B T} \end{pmatrix}$$

Note: Diagonal (no off-diagonal elements) → no coherence, pure statistical mixture.

## Magnetization Calculation
Magnetization M = average magnetic moment of ensemble:
$$M = N\langle\mu_z\rangle = N \cdot \text{tr}(\mu \hat{S}_z \hat{\rho})$$

Since μ = geℏ/(4mₑc) and Ŝᵤ = (ℏ/2)σᵤ:
$$\hat{S}_z = \frac{\hbar}{2}\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$$

**Matrix product**:
$$\hat{S}_z\hat{\rho} = \frac{\hbar}{2Z}\begin{pmatrix} e^{\mu B/k_B T} & 0 \\ 0 & -e^{-\mu B/k_B T} \end{pmatrix}$$

**Trace**:
$$\langle S_z\rangle = \frac{\hbar}{2Z}\left(e^{\mu B/k_B T} - e^{-\mu B/k_B T}\right)$$

$$= \frac{\hbar}{2} \frac{e^{\mu B/k_B T} - e^{-\mu B/k_B T}}{e^{\mu B/k_B T} + e^{-\mu B/k_B T}}$$

$$= \frac{\hbar}{2}\tanh(\mu B/k_B T)$$

**Magnetization**:
$$M = N\mu\langle S_z\rangle / (\hbar/2) = N\mu\tanh(\mu B/k_B T)$$

## High Temperature Limit (Curie's Law)
When μB/kᴮT ≪ 1 (thermal energy ≫ magnetic energy):

Use approximation: tanh(x) ≈ x for x ≪ 1

$$M \approx N\mu \frac{\mu B}{k_B T} = \frac{N\mu^2 B}{k_B T}$$

Define Curie constant: C = Nμ²/kᴮ

$$M = \frac{CB}{T}$$

This is **Curie's law** for paramagnetism: M ∝ 1/T

**Physical interpretation**: At high temperature, thermal fluctuations randomize spins. Only small magnetic ordering remains, decreasing with temperature.

## Low Temperature Limit
When μB/kᴮT ≫ 1:

tanh(x) → 1 for x ≫ 1

$$M \approx N\mu$$

**Physical interpretation**: Almost all spins align with field (in ground state |+z⟩). Maximal magnetization.

## Temperature Dependence
| Regime | Condition | M behavior | Physics |
|--------|-----------|------------|---------|
| Low T | kᴮT ≪ μB | M → Nμ | All spins aligned |
| High T | kᴮT ≫ μB | M ∝ 1/T | Thermal randomization |

## Key Results
- Density operator is diagonal in energy basis (no coherence)
- tr ρ² = [tanh²(μB/kᴮT) + (1-tanh²)] / [calculation needed] < 1 (mixed state)
- Curie's law emerges naturally from thermal density operator
- Historical: Pierre Curie discovered 1/T law experimentally before quantum mechanics!

## Related
- [[Thermal Equilibrium and Density Operator]]
- [[Density Operator Mixed State]]
- [[Hamiltonian Operator]]
- [[Magnetic Moment]]