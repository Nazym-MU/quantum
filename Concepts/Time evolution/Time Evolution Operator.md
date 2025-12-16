**Definition:** Unitary operator Û(t) that translates a quantum state forward in time:
$$\ket{\psi(t)} = \hat{U}(t)\ket{\psi(0)}$$

## Properties
- **Unitary**: $Û^†Û = I$ (preserves probability/normalization)
- **Composition**: $Û(t_2)Û(t_1) = Û(t₂ + t₁$) (time translations compose)
- **Initial condition**: $Û(0) = I$ (no evolution at t=0)
- **Infinitesimal form**: $Û(dt) = 1 - \frac{i}{\hbar}\hat{H}dt$ for small dt.

## Connection to Hamiltonian
When Ĥ is time-independent:
$$\hat{U}(t) = e^{-i\hat{H}t/\hbar}$$

## Related
- [[Hamiltonian Operator]]
- [[Schrödinger Equation (Time-Dependent)]]