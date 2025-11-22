Physical requirement that wave functions must satisfy for bound states.

## Mathematical Condition

For particle confined to region, wave function must satisfy:
$$\int_{-\infty}^{\infty} |\psi(x)|^2 dx = 1$$

More generally, integral must be **finite** (can then normalize).

## Physical Meaning

|ψ(x)|² is probability density to find particle at position x.

For meaningful probability interpretation:
- Total probability must equal 1 (particle exists somewhere)
- Cannot have infinite total probability
- Wave function cannot "blow up" at infinity

## Asymptotic Requirements

For normalizability, wave function must decay as |x| → ∞:
$$\psi(x) \xrightarrow{|x| \to \infty} 0 \text{ sufficiently fast}$$

**Acceptable behaviors**:
- Exponential decay: e^(-|x|)
- Gaussian: e^(-x²)
- Power law with sufficient decay: 1/x³ (borderline: 1/x²)

**Unacceptable behaviors**:
- Exponential growth: e^(|x|)
- Constants: ψ = A (doesn't decay)
- Oscillations without decay: sin(kx) (spreads probability to infinity)

## Harmonic Oscillator Example

Position-space differential equation suggests asymptotic solutions:
$$\psi(y) \sim e^{\pm y^2/2}$$

- e^(-y²/2): Normalizable ✓ (Gaussian decay)
- e^(+y²/2): Not normalizable ✗ (exponential growth)

This rejects positive exponential.

With power series h(y), if series doesn't terminate:
$$h(y) \sim e^{y^2} \implies \psi(y) = h(y)e^{-y^2/2} \sim e^{y^2/2}$$

Not normalizable! Forces series termination → energy quantization.

Derivation: [[Series Termination and Energy Quantization]]

## Bound vs Unbound States

**Bound states** (E < V(∞)):
- Must be normalizable
- Discrete energy spectrum
- Examples: harmonic oscillator, infinite well, finite well

**Unbound states** (E > V(∞)):
- Not normalizable (extend to infinity)
- Continuous energy spectrum
- Examples: free particle, scattering states

See: [[Bound States]], [[Unbound States]]

## Normalization Process

If ψ satisfies Schrödinger equation but ∫|ψ|²dx = C ≠ 1:

**Normalize**: ψ_normalized = ψ/√C

Normalized function has ∫|ψ_normalized|²dx = 1.

## Connection to Energy Quantization

For bound states in potential well:
1. Schrödinger equation has solutions for all energies E
2. Most solutions blow up at infinity (non-normalizable)
3. Only special energies Eₙ give normalizable solutions
4. These are the allowed energy levels (quantization)

**Examples**:
- [[Harmonic Oscillator]]: Eₙ = (n + ½)ℏω
- [[Infinite Square Well (Particle in a Box)]]: Eₙ = n²π²ℏ²/2mL²
- [[Finite Square Well]]: Discrete spectrum determined by transcendental equation

## Related
- [[Asymptotic Solution for Harmonic Oscillator]]
- [[Series Termination and Energy Quantization]]  
- [[Bound States]]
- [[Boundary Conditions for Wave Functions]]
- [[Wave Function]]