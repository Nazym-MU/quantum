# Off-Diagonal Elements and Coherence

Off-diagonal elements in a density matrix distinguish quantum superposition from classical statistical mixture.
## Pure State Superposition
For |ψ⟩ = c₁|1⟩ + c₂|2⟩:
$$\hat{\rho} = |\psi\rangle\langle\psi| = \begin{pmatrix} |c_1|^2 & c_1c_2^* \\ c_1^*c_2 & |c_2|^2 \end{pmatrix}$$
**Off-diagonal elements**: ρ₁₂ = c₁c₂* encodes:
- Magnitude: |c₁||c₂| (overlap strength)
- Phase: relative phase between c₁ and c₂
### Example: |+y⟩ in Sᵤ basis
$$|+y\rangle = \frac{1}{\sqrt{2}}(|+z\rangle + i|-z\rangle)$$
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$

The **-i** and **i** off-diagonal elements encode the **i phase** between |+z⟩ and |-z⟩ components.

### Example: |+x⟩ in Sᵤ basis
$$|+x\rangle = \frac{1}{\sqrt{2}}(|+z\rangle + |-z\rangle)$$
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix}$$

The **real positive** off-diagonal elements reflect the **real positive** coefficients.

## Mixed State: No Coherence
For mixed state ρ = Σₖ pₖ|ψₖ⟩⟨ψₖ| with orthogonal |ψₖ⟩:
$$\hat{\rho} = \begin{pmatrix} p_1 & 0 \\ 0 & p_2 \end{pmatrix}$$

**Zero off-diagonal elements** → no quantum coherence between states.

### Example: 50-50 Mix of |±z⟩
$$\hat{\rho} = \frac{1}{2}|+z\rangle\langle+z| + \frac{1}{2}|-z\rangle\langle-z| = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$$

No off-diagonal elements → pure classical probability, no quantum interference.

## Physical Significance: Quantum Coherence
**Quantum coherence** = ability to show interference effects in measurements.

- **Superposition** (|ψ⟩ = c₁|1⟩ + c₂|2⟩): Off-diagonal elements present → interference possible
- **Mixture** (50% |1⟩, 50% |2⟩): Zero off-diagonal → no interference

### Experimental Test
Measure in a basis rotated from {|1⟩, |2⟩}:
- **Superposition**: Shows interference fringes (oscillations in probabilities)
- **Mixture**: Shows only statistical averages (no oscillations)

## Decoherence
Environmental interactions cause off-diagonal elements to decay:
$$\rho_{12}(t) = \rho_{12}(0) e^{-\gamma t}$$

This is **decoherence**: quantum coherence → classical mixture. System loses ability to interfere.

## Mathematical Reason
Off-diagonal elements come from cross-terms in outer product:
$$|\psi\rangle\langle\psi| = (c_1|1\rangle + c_2|2\rangle)(c_1^*\langle 1| + c_2^*\langle 2|)$$
$$= |c_1|^2|1\rangle\langle 1| + c_1c_2^*|1\rangle\langle 2| + c_1^*c_2|2\rangle\langle 1| + |c_2|^2|2\rangle\langle 2|$$

The middle two terms (c₁c₂*|1⟩⟨2| and c₁*c₂|2⟩⟨1|) create off-diagonal matrix elements.

For mixed state:
$$\hat{\rho} = p_1|1\rangle\langle 1| + p_2|2\rangle\langle 2|$$
No cross-terms → no off-diagonal elements.

## Summary
| State Type | Off-Diagonal Elements | Physical Meaning |
|------------|----------------------|------------------|
| Pure superposition | Non-zero (complex) | Quantum coherence, interference possible |
| Mixed state | Zero | Classical statistics, no interference |

## Related
- [[Density Operator Pure State]]
- [[Density Operator Mixed State]]
- [[Quantum States and Amplitudes]]
- [[Measurement and State Collapse]]