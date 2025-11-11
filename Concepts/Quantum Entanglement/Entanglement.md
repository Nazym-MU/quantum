## Definition
A quantum state is entangled if it **cannot be written as a product of individual particle states**. For two particles, if the state cannot be factored as |ψ⟩ = |ψ₁⟩ ⊗ |ψ₂⟩, then the particles are entangled.

## Key Property
In an entangled state, the particles do not have individual definite quantum states. Only the combined two-particle state is well-defined. Neither particle has its own separate wavefunction.

## Test for Entanglement
**Product state (NOT entangled):**
$$|+z\rangle_1|+z\rangle_2 = |+z\rangle_1 \otimes |+z\rangle_2$$
Can be written as (particle 1's state) ⊗ (particle 2's state).

**Entangled state:**
$$|0,0\rangle = \frac{1}{\sqrt{2}}(|+z\rangle_1|-z\rangle_2 - |-z\rangle_1|+z\rangle_2)$$
Cannot be factored into separate states for particles 1 and 2.

## Measurement Correlations
When you measure one particle in an entangled pair:
- The measurement outcome is random (50/50 for spin-1/2)
- The other particle's measurement outcome is instantly correlated
- This is NOT causation—the particles were never independent to begin with

The correlation exists because the two-particle state constrains both measurements together, not because one measurement "causes" the other to collapse.

## Examples

**Entangled:**
- Singlet state: $\frac{1}{\sqrt{2}}(|+z\rangle_1|-z\rangle_2 - |-z\rangle_1|+z\rangle_2)$
- All [[Bell State Measurement]] basis states

**Not Entangled (Product States):**
- $|+z\rangle_1|+z\rangle_2$ (both spin-up)
- $\frac{1}{2}(|+x\rangle_1 + |-x\rangle_1)(|+z\rangle_2 + |-z\rangle_2)$ (expands to product)

## How to Check
Expand the state fully. If you can group all terms involving particle 1 separately from all terms involving particle 2, it's a product state (not entangled). If the particles are mixed together in the superposition, they're entangled.

## Related Concepts
- [[Singlet State]]
- [[EPR Pair]]
- [[Bell State Measurement]]
- [[Quantum Teleportation]]
- [[EPR Paradox]]