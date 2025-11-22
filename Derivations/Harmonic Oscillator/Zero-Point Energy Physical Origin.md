Detailed explanation of why the [[Harmonic Oscillator]] ground state has non-zero energy E₀ = ℏω/2.
## The Classical Impossibility
Classically, the lowest energy state occurs when:
- Particle at rest: p = 0 → kinetic energy = 0
- Spring unstretched: x = 0 → potential energy = 0
- Total energy: E = 0
**This is forbidden in quantum mechanics.**
## Quantum Mechanical Constraint
The fundamental [[Position-Momentum Commutator]] requires:
$$[\hat{x}, \hat{p}_x] = i\hbar$$
This commutation relation leads to the [[Uncertainty|Heisenberg uncertainty relation]]:
$$\Delta x \cdot \Delta p_x \geq \frac{\hbar}{2}$$
## Energy in Terms of Uncertainties
For any quantum state:
$$E = \frac{\langle p_x^2\rangle}{2m} + \frac{1}{2}m\omega^2\langle x^2\rangle$$

For energy eigenstates, ⟨x⟩ = 0 and ⟨pₓ⟩ = 0 (proven in [[Harmonic Oscillator Position Uncertainty]] and [[Harmonic Oscillator Momentum Uncertainty]]).
Therefore:
$$E = \frac{\langle\Delta p_x^2\rangle}{2m} + \frac{1}{2}m\omega^2\langle\Delta x^2\rangle$$

## The Tradeoff

Nature must balance two competing requirements:

1. **Minimize potential energy**: Localize particle near x = 0
   - Small Δx → Large Δp (by uncertainty relation)
   - Increases kinetic energy

2. **Minimize kinetic energy**: Reduce momentum uncertainty
   - Small Δp → Large Δx (by uncertainty relation)
   - Increases potential energy

Neither extreme works.
## Ground State Calculation

From [[Harmonic Oscillator Position Uncertainty]] and [[Harmonic Oscillator Momentum Uncertainty]]:

For the ground state (n = 0):
$$\langle\Delta x^2\rangle_0 = \frac{\hbar}{2m\omega}$$

$$\langle\Delta p_x^2\rangle_0 = \frac{m\omega\hbar}{2}$$

## Ground State Energy

Substitute into energy formula:
$$E_0 = \frac{\langle\Delta p_x^2\rangle_0}{2m} + \frac{1}{2}m\omega^2\langle\Delta x^2\rangle_0$$

$$= \frac{m\omega\hbar/2}{2m} + \frac{1}{2}m\omega^2 \cdot \frac{\hbar}{2m\omega}$$

$$= \frac{\omega\hbar}{4} + \frac{\omega\hbar}{4}$$

$$= \frac{\hbar\omega}{2}$$

## Minimum Uncertainty State

The ground state achieves:
$$\Delta x \cdot \Delta p_x = \sqrt{\frac{\hbar}{2m\omega}} \cdot \sqrt{\frac{m\omega\hbar}{2}} = \frac{\hbar}{2}$$

This **saturates** the uncertainty relation - the ground state has the minimum allowed uncertainty product.

## Why Gaussian?

The [[Ground State Wave Function Derivation]] shows ⟨x|0⟩ is Gaussian. This is the only wave function shape that:
1. Minimizes the uncertainty product ΔxΔp
2. Has equal contributions from kinetic and potential energy
3. Is stable (stationary state)

## Physical Consequences

### Helium Won't Solidify at 1 atm

Helium atoms have:
- Small mass m → Large Δx for given energy
- Weak inter-atomic forces → Small ω → Large Δx

Even at T = 0, the zero-point motion (Δx ≈ √(ℏ/mω)) is large enough that atoms can't localize into a crystal lattice at atmospheric pressure.

Need P ≥ 25 atm to compress system enough (increase ω) to reduce Δx and allow solidification.

### Temperature and Excited States

At temperature T, thermal energy kᴃT populates excited states with n ∼ kᴃT/(ℏω).

From [[Harmonic Oscillator Position Uncertainty]]:
$$\Delta x \propto \sqrt{2n+1}$$

As T increases → n increases → Δx increases → solid melts when Δx becomes comparable to lattice spacing.

## Summary

The zero-point energy is:
1. **Unavoidable**: Consequence of [x̂, p̂] = iℏ
2. **Optimized**: Ground state minimizes energy subject to uncertainty relation
3. **Observable**: Affects phase transitions (e.g., helium's unusual properties)

## Related

- [[Zero-Point Energy]]
- [[Harmonic Oscillator Position Uncertainty]]
- [[Harmonic Oscillator Momentum Uncertainty]]
- [[Uncertainty]]
- [[Position-Momentum Commutator]]