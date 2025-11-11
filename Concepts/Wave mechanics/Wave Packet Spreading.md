## Free Particle Time Evolution
For a free particle with Hamiltonian Ĥ = p̂²/(2m), momentum eigenstates are energy eigenstates:

$$E = \frac{p^2}{2m}$$

Time evolution:
$$|\psi(t)\rangle = \int dp \, e^{-ip^2t/(2m\hbar)}|p\rangle\langle p|\psi(0)\rangle$$

## Gaussian Wave Packet Spreading

**Initial state (t=0):**
$$\psi(x,0) = \frac{1}{(\pi a^2)^{1/4}}e^{-x^2/(2a^2)}$$
$$\Delta x(0) = \frac{a}{\sqrt{2}}$$

**Time-evolved state:**
$$\psi(x,t) = \frac{1}{\sqrt{\pi[a + i\hbar t/(ma)]}}e^{-x^2/\{2a^2[1+(i\hbar t/ma^2)]\}}$$

**Position uncertainty grows:**
$$\Delta x(t) = \frac{a}{\sqrt{2}}\sqrt{1 + \frac{\hbar^2 t^2}{m^2 a^4}}$$

## Characteristic Time Scale
Define spreading time τ:
$$\tau = \frac{ma^2}{\hbar}$$

For t << τ: No significant spreading (Δx ≈ a/√2)
For t >> τ: Linear spreading (Δx ≈ ℏt/(√2 ma))

## Physical Interpretation
- Different momentum components move at different velocities
- Momentum uncertainty Δp causes velocity spread: Δv = Δp/m
- Wave packet disperses like classical particles with velocity distribution
- Smaller initial Δx → larger Δp → faster spreading

## Momentum Uncertainty Unchanged
$$\Delta p(t) = \Delta p(0) = \frac{\hbar}{\sqrt{2}a}$$

Momentum uncertainty is constant because free particle Hamiltonian commutes with p̂.

## Examples
**Macroscopic (m=1g, a=0.1cm):** τ ≈ 10²⁵ s (no observable spreading)
**Electron (m=9×10⁻³¹kg, a=10⁻⁸cm):** τ ≈ 10⁻¹⁶ s (rapid spreading)