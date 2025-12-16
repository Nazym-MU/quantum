Potential step:
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & x > 0 \end{cases}$$

Particle incident from left with energy E.
## Wave Function Form
### Region x < 0
$$\psi(x) = Ae^{ikx} + Be^{-ikx}$$
where k = √(2mE)/ℏ
- Ae^(ikx): incident wave (rightward)
- Be^(-ikx): reflected wave (leftward)
### Region x > 0: Case E > V₀
$$\psi(x) = Ce^{ik_0x}$$
where k₀ = √(2m(E-V₀))/ℏ
Transmitted wave only (D = 0 since no source at x → +∞).
### Region x > 0: Case E < V₀
$$\psi(x) = Ce^{-qx}$$
where q = √(2m(V₀-E))/ℏ
Evanescent wave (decaying exponential, not propagating).
## Boundary Conditions at x = 0
1. Continuity of ψ: A + B = C
2. Continuity of ∂ψ/∂x: ik(A - B) = ik₀C (for E > V₀) or ik(A - B) = -qC (for E < V₀)
## Results for E > V₀
$$B = \frac{k - k_0}{k + k_0}A$$
$$C = \frac{2k}{k + k_0}A$$
### [[Reflection Coefficient]]
$$R = \left|\frac{B}{A}\right|^2 = \left(\frac{k - k_0}{k + k_0}\right)^2$$
### [[Transmission Coefficient]]
$$T = \frac{k_0}{k}\left|\frac{C}{A}\right|^2 = \frac{4kk_0}{(k + k_0)^2}$$
Verify: R + T = 1
### Classical vs Quantum
- Classical: R = 0 (particle simply slows down)
- Quantum: R ≠ 0 (partial reflection at interface despite E > V₀)
## Results for E < V₀
$$B = \frac{k + iq}{k - iq}A$$
$$C = \frac{2k}{k - iq}A$$

Note: |B|² = |A|² since |(k+iq)/(k-iq)|² = 1
### Scattering Probabilities
$$R = 1, \quad T = 0$$

Wave penetrates distance ~1/q but carries no [[Probability Current]] (j_trans = 0).
## Physical Interpretation
Step potential shows:
- Quantum reflection even when E > V₀
- Wave penetration but no transmission when E < V₀
- Smooth matching at boundary via ψ and ∂ψ/∂x continuity
## Derivation
See [[Step Potential Solution]] for complete calculation.
## Related
- [[Unbound States]]
- [[Potential Barrier Scattering]]
- [[Reflection Coefficient]]
- [[Transmission Coefficient]]