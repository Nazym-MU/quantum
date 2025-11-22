Operator that performs spatial inversion (reflection through origin) on quantum states.

## Definition

$$\hat{\Pi}|x\rangle = |-x\rangle$$

Acts on position eigenstates by flipping sign of position.

## Action on Wave Functions

For arbitrary state |ψ⟩:
$$\langle x|\hat{\Pi}|\psi\rangle = \psi(-x)$$

Derivation: [[Parity Operator Action]]

**Meaning**: Parity operator evaluates wave function at reflected position.

## Eigenvalues and Eigenstates

Since Π̂² = 1, eigenvalues are λ = ±1.

Eigenvalue equation:
$$\hat{\Pi}|\psi\rangle = \lambda|\psi\rangle$$
$$\psi(-x) = \lambda\psi(x)$$

### λ = +1: Even Parity
Wave function unchanged under reflection:
$$\psi(-x) = \psi(x)$$

Examples: cos(x), x², e^(-x²), all [[Even and Odd Functions|even functions]]

### λ = -1: Odd Parity  
Wave function changes sign under reflection:
$$\psi(-x) = -\psi(x)$$

Examples: sin(x), x, x³, all [[Even and Odd Functions|odd functions]]

## Hermiticity

Π̂ is Hermitian (observable). Its eigenvalues ±1 are real, representing measurable parity.

## Commutation with Hamiltonian

For potentials with inversion symmetry V(-x) = V(x):
$$[\hat{\Pi}, \hat{H}] = 0$$

Derivation: [[Parity-Hamiltonian Commutation]]

**Consequence**: Energy eigenstates have definite parity (are simultaneous eigenstates of Ĥ and Π̂).

Examples:
- ✓ Harmonic oscillator: V(x) = ½mω²x²
- ✓ Infinite square well centered at origin
- ✗ Linear potential: V(x) = mgx (breaks symmetry)

## Harmonic Oscillator Application

Energy eigenstates |n⟩ have parity (-1)ⁿ:
- |0⟩: even (H₀ = 1)
- |1⟩: odd (H₁ = y)
- |2⟩: even (H₂ = 2y²-1)
- ...

See: [[Hermite Polynomials]], [[First Three Hermite Polynomials]]

## Selection Rules

Parity conservation affects which transitions are allowed. 

For electric dipole transitions ∝ ⟨f|x̂|i⟩:
- x̂ has odd parity
- ⟨f|x̂|i⟩ ≠ 0 only if states have opposite parity
- Even ↔ odd allowed, even ↔ even forbidden

## Physical Meaning

**Parity symmetry**: Laws of physics unchanged under spatial inversion

In quantum mechanics, if Hamiltonian has parity symmetry, energy eigenstates can be chosen with definite parity. This constrains solutions before solving differential equations.

## Related
- [[Even and Odd Functions]]
- [[Parity Operator Action]]
- [[Parity-Hamiltonian Commutation]]
- [[Compatible and Incompatible Observables]]
- [[Week 11.2 - Position Space Solution and Parity]]