One-dimensional differential equation for the radial wave function in a central potential.
For central potential V(r), energy eigenvalue equation in position space:

$$\left[-\frac{\hbar^2}{2\mu} \left(\frac{\partial^2}{\partial r^2} + \frac{2}{r} \frac{\partial}{\partial r}\right) + \frac{\hat L^2}{2\mu r^2} + V(r)\right]⟨r|E, l, m⟩ = E⟨r|E, l, m⟩$$
Wave function factorizes:
$$⟨r|E, l, m⟩ = R(r)Θ(θ)Φ(\phi)$$
The angular part is determined by $l$ and $m$ (spherical harmonics). The energy depends only on $r$.
## Radial Equation (Standard Form)
$$\left[-\frac{\hbar^2}{2\mu} \left(\frac{\partial^2}{\partial r^2} + \frac{2}{r} \frac{\partial}{\partial r}\right) + \frac{\hat L^2}{2\mu r^2} + V(r)\right]R(r) = ER(r)$$
## Simplified Form Using u(r)
Define: $R(r) = u(r)/r$
Substituting and simplifying:
$$\left[-\frac{\hbar^2}{2\mu} \frac{d^2}{d r^2} + \frac{l(l+1)\hbar^2}{2\mu r^2} + V(r)\right]u(r) = Eu(r)$$
This has the form of a 1D Schrödinger equation with effective potential.
Energy doesn't depend on $m$ (magnetic quantum number). This manifests rotational invariance. All $2l+1$ states with same $E$ and $l$ but different $m$ are degenerate.
## Boundary Conditions
- **r → 0**: u(0) = 0 (ensures R(r) = u(r)/r is finite)
- **r → ∞**: u(r) → 0 for bound states (normalizability)

Related: [[Effective Potential in Central Force Problem]], [[Reduction to One-Dimensional Radial Equation]], [[Radial Momentum Operator]]
