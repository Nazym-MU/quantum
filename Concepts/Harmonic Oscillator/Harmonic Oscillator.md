A quantum system with potential V(x) = ½mω²x² where the particle experiences a restoring force proportional to displacement.
## Physical Significance
The harmonic oscillator is fundamental because near any potential minimum at x₀, a Taylor expansion gives:
$$V(x) \approx V(x_0) + \frac{1}{2}k(x-x_0)^2$$
where k = (d²V/dx²)|ₓ₌ₓ₀ > 0.
Setting the zero of energy at V(x₀) = 0 and shifting coordinates gives V(x) = ½kx² = ½mω²x² with ω = √(k/m).
**Examples**: molecular vibrations, atoms in solids, electromagnetic field modes.
## Hamiltonian

$$\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2$$

Uses the fundamental commutator [[Position-Momentum Commutator]]: [x̂,p̂ₓ] = iℏ.

## Energy Spectrum

The energy eigenvalues are:
$$E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0,1,2,\ldots$$

**Key features**:
- Discrete, evenly spaced levels with spacing ℏω
- [[Zero-Point Energy]] E₀ = ½ℏω (cannot be zero due to uncertainty principle)
- No upper bound on energy

Derivation: [[Number Operator Eigenvalue Derivation]]

## Solution Methods

Two approaches:
1. **Operator method** (sections 7.2-7.3): Uses [[Ladder Operators]] â, â† 
2. **Wave mechanics** (section 7.4): Solves differential equation for ⟨x|n⟩

The operator method is more general and extends to quantum field theory.

## Key Operators

- [[Number Operator]]: N̂ = â†â with N̂|n⟩ = n|n⟩
- [[Ladder Operators]]: â (lowering) and â† (raising)
- Hamiltonian: Ĥ = ℏω(N̂ + ½)

## Classical Limit

For large n, the quantum spacing ℏω becomes negligible compared to total energy E ≈ nℏω, recovering classical continuous spectrum.

Classical turning points: x_n = ±√((2n+1)ℏ/mω) where all energy is potential.

## Related Concepts

- [[Ladder Operators]]
- [[Number Operator]]
- [[Zero-Point Energy]]
- [[Harmonic Oscillator Wave Functions]]