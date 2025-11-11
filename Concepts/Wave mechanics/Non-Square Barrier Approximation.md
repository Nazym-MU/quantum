# Non-Square Barrier Approximation

## Context
For barriers where V(x) varies continuously rather than in steps, exact solutions are typically unavailable. An approximation method exists for slowly-varying potentials.

## WKB Approximation Result

For a non-square barrier where E < V(x) in region [x₁, x₂]:
$$T \approx \exp\left(-2\int_{x_1}^{x_2} q(x)\,dx\right)$$

where:
$$q(x) = \frac{\sqrt{2m[V(x) - E]}}{\hbar}$$

Integration limits x₁ and x₂ are the classical turning points where E = V(x).

## Derivation Intuition

1. Approximate smooth barrier by sequence of thin square barriers
2. For each thin barrier of width δx:
   $$T_i \approx e^{-2q_i \delta x}$$
3. Total transmission is product:
   $$T = \prod_i T_i$$
4. Take logarithm:
   $$\ln T = \sum_i \ln T_i \approx -2\sum_i q_i\delta x$$
5. In continuum limit, sum → integral:
   $$\ln T \approx -2\int q(x)\,dx$$

## Validity Requirements

- Barrier width much larger than penetration depth
- Potential varies slowly (∂V/∂x small)
- qa >> 1 at each point (WKB approximation)
- Breaks down near turning points but still gives reasonable results

## Physical Applications

### Field Emission from Metals
Electrons tunnel through triangular barrier created by:
- Metal work function
- Applied electric field

Transmission determines emission current.

### Alpha Decay
Alpha particles tunnel through Coulomb barrier of nucleus. Transmission coefficient determines decay rate.

### General Tunneling Problems
Any slowly-varying potential barrier where E < V(x) in some region.

## Relation to Square Barrier

For square barrier with constant V₀:
$$q(x) = q = \text{constant}$$
$$\int_0^a q\,dx = qa$$

Recovers: T ∝ e^(-2qa), consistent with [[Barrier Tunneling Solution]].

---

## Summary
The WKB method extends tunneling calculations to realistic (non-square) barriers. Result depends on integral of √[V(x)-E] over classically forbidden region—larger integral means more suppression.

## Related
- [[Quantum Tunneling]]
- [[Potential Barrier Scattering]]
- [[Transmission Coefficient]]