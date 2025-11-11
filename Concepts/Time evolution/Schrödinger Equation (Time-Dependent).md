**Definition:** Fundamental equation governing how quantum states evolve in time.

$$i\hbar \frac{\partial}{\partial t}\ket{\psi(t)} = \hat{H}\ket{\psi(t)}$$
## Interpretation
- Left side: Rate of change of the state (how fast ψ is evolving)
- Right side: Hamiltonian acting on the state (energy tells you how to evolve)
- The factor i/ℏ sets the units and ensures unitary evolution
## Derivation
Obtained from the infinitesimal form of the [[Time Evolution Operator]]:
$$\hat{U}(dt) = I - \frac{i}{\hbar}\hat{H}dt$$## When Ĥ is Time-Independent
Can integrate to get:
$$\ket{\psi(t)} = e^{-i\hat{H}t/\hbar}\ket{\psi(0)}$$
This is the formal solution connecting to Û(t).
## Key Properties
- Not a wave equation (despite the name "wave function")
- First-order in time (unlike classical wave equations)
- Linear equation (superposition principle holds)
- Deterministic (knowing ψ(0) determines ψ(t) for all t)
## Related
- [[Hamiltonian Operator]]
- [[Time Evolution Operator]]
- [[Schrödinger Equation (Time-Independent)]]