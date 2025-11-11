# Potential Barrier Scattering

## Setup
Square potential barrier:
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & 0 < x < a \\ 0 & x > a \end{cases}$$

Particle incident from left with energy E < V₀ (classically forbidden to cross).

## Wave Function Form

### Region x < 0
$$\psi(x) = Ae^{ikx} + Be^{-ikx}$$
where k = √(2mE)/ℏ

### Region 0 < x < a  
$$\psi(x) = Fe^{qx} + Ge^{-qx}$$
where q = √(2m(V₀-E))/ℏ

Both exponentials needed since barrier has finite width. Cannot eliminate either F or G.

### Region x > a
$$\psi(x) = Ce^{ikx}$$

Transmitted wave only (no source from right).

## Boundary Conditions

### At x = 0
1. A + B = F + G
2. ik(A - B) = q(F - G)

### At x = a
3. Fe^(qa) + Ge^(-qa) = Ce^(ika)
4. q(Fe^(qa) - Ge^(-qa)) = ikCe^(ika)

Four equations, five unknowns (A, B, C, F, G). Fix A (incident amplitude), solve for others.

## Transmission Coefficient

### Exact Result
$$T = \frac{1}{1 + \frac{(k^2 + q^2)^2}{4k^2q^2}\sinh^2(qa)}$$

This is the [[Quantum Tunneling]] probability.

### Wide Barrier Limit (qa >> 1)
Using sinh(qa) ≈ e^(qa)/2:
$$T \approx \frac{16k^2q^2}{(k^2+q^2)^2}e^{-2qa}$$

Dominant behavior: **exponential suppression** T ∝ e^(-2qa).

### Physical Dependence
- Thicker barrier (larger a): smaller T (exponential decay)
- Higher barrier (larger V₀): larger q, smaller T  
- Higher energy E: smaller q, larger T

## Classical vs Quantum
- Classical: T = 0 (particle cannot cross barrier if E < V₀)
- Quantum: T ≠ 0 (tunneling occurs)

## Reflection Coefficient
$$R = 1 - T < 1$$

Not total reflection due to tunneling.

## Why Tunneling Occurs
Wave function penetrates barrier as evanescent wave (∝ e^(-qx)). For finite width a, amplitude remains finite at x = a, allowing nonzero transmission to x > a region where wave becomes propagating again.

## Derivation
See [[Barrier Tunneling Solution]] for complete boundary condition matching.

## Related
- [[Quantum Tunneling]]
- [[Potential Step Scattering]]
- [[Transmission Coefficient]]
- [[Unbound States]]