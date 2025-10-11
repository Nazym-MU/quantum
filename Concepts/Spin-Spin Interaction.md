## Physical Origin

Magnetic interaction between two spinning particles, each with its own magnetic moment.
The energy of interaction depends on:
- The magnetic moments of both particles
- The intrinsic spins of both particles (since $\mu \propto S$)
- The spatial separation and wave function
## Simplified Form for ℓ = 0 States
For states with **zero orbital angular momentum** (s-orbitals, like hydrogen ground state):
$$\hat{H}_{\text{spin-spin}} = \frac{A}{\hbar^2}\hat{S}_1 \cdot \hat{S}_2$$
where:
- $\hat{S}_1 \cdot \hat{S}_2 = \hat{S}_{1x}\hat{S}_{2x} + \hat{S}_{1y}\hat{S}_{2y} + \hat{S}_{1z}\hat{S}_{2z}$ (dot product of spin operators)
- $A$ = coupling constant (energy units, determined experimentally)
- Factor $\hbar^2$ ensures dimensional consistency
---
The full spin-spin Hamiltonian from Maxwell's equations is complicated and depends on the spatial wave function. For ℓ = 0 (spherically symmetric), it simplifies to this clean operator form.
## Key Properties
- The interaction is **symmetric** under particle exchange: $\hat{S}_1 \cdot \hat{S}_2 = \hat{S}_2 \cdot \hat{S}_1$
- Sign of A:
	- If $A > 0$: Lower energy when spins are **antiparallel** (opposite directions)
	- If $A < 0$: Lower energy when spins are **parallel** (same direction)
For hydrogen hyperfine: $A > 0$, so the singlet state (antiparallel spins) has lower energy.
## Operator Identity
For computing matrix elements: $$2\hat{S}_1 \cdot \hat{S}_2 = \hat{S}_{1+}\hat{S}_{2-} + \hat{S}_{1-}\hat{S}_{2+} + 2\hat{S}_{1z}\hat{S}_{2z}$$
- Diagonal terms come from $\hat{S}_{1z}\hat{S}_{2z}$
- Off-diagonal terms come from ladder operators
- Easy to evaluate matrix elements in the $|s_{1z}, s_{2z}\rangle$ basis
## Relation to Total Spin
$$\hat{S}_1 \cdot \hat{S}_2 = \frac{1}{2}[\hat{S}^2_{\text{total}} - \hat{S}^2_1 - \hat{S}^2_2]$$
## Related Concepts

- [[Two-Particle Spin Systems]]
- [[Raising and Lowering Operators]]
- [[Magnetic moment]]