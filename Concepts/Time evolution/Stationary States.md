**Definition:** Energy eigenstates of the Hamiltonian that evolve only by an overall phase factor.
## Mathematical Form
If $Ĥ\ket{E} = E\ket{E}$, then:
$$\ket{\psi(t)} = e^{-iEt/\hbar}\ket{E}$$
## Key Property
**All expectation values are time-independent** for stationary states:
$$\braket{\psi(t)|\hat{A}|\psi(t)} = \braket{E|\hat{A}|E}$$

The phase factor $e^{-iEt/ℏ}$ cancels when computing $⟨ψ(t)|Â|ψ(t)⟩$.
## Why "Stationary"?
- Physical observables don't change with time
- Only the overall phase evolves (not observable)
- Probability distributions remain constant
## Contrast: Superposition States
If $\ket{\psi(0)} = c₁\ket{E₁} + c₂\ket{E₂}$ with E₁ ≠ E₂:
- Relative phase evolves: $e^{-i(E₂-E₁)t/ℏ}$
- Expectation values oscillate with frequency ω = (E₂-E₁)/ℏ
- NOT a stationary state
## Related
- [[Schrödinger Equation (Time-Independent)]]