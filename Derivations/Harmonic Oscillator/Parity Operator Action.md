## Definition

The **parity operator** Π̂ inverts position through the origin:
$$\hat{\Pi}|x\rangle = |-x\rangle$$

## Action on Wave Functions
Consider arbitrary state |ψ⟩. Project onto position:
$$\langle x|\hat{\Pi}|\psi\rangle = \langle x|(\hat{\Pi}|\psi\rangle)$$
Using Π̂|x⟩† = ⟨x|Π̂† = ⟨-x| (since Π̂ is Hermitian):
$$\langle x|\hat{\Pi}|\psi\rangle = \langle -x|\psi\rangle = \psi(-x)$$
$$\langle x|\hat{\Pi}|\psi\rangle = \psi(-x)$$

**Meaning**: Parity operator flips x → -x in wave function.

## Eigenvalue Equation

If |ψ⟩ is eigenstate of Π̂:
$$\hat{\Pi}|\psi\rangle = \lambda|\psi\rangle$$

Project onto position:
$$\langle x|\hat{\Pi}|\psi\rangle = \lambda\langle x|\psi\rangle = \lambda\psi(x)$$

But from above, ⟨x|Π̂|ψ⟩ = ψ(-x), so:

**Result (Eq. 7.119)**:
$$\psi(-x) = \lambda\psi(x)$$

## Eigenvalues

Apply parity twice:
$$\hat{\Pi}^2|x\rangle = \hat{\Pi}(|-x\rangle) = |x\rangle$$

So Π̂² = 1 (identity operator).

If Π̂|ψ⟩ = λ|ψ⟩, then:
$$\hat{\Pi}^2|\psi\rangle = \lambda^2|\psi\rangle = |\psi\rangle$$

Therefore λ² = 1, giving **λ = ±1**.

### Even Functions (λ = +1)
$$\psi(-x) = +\psi(x)$$

Examples: 1, x², cos(x), e^(-x²)

### Odd Functions (λ = -1)
$$\psi(-x) = -\psi(x)$$

Examples: x, x³, sin(x), xe^(-x²)

## Physical Interpretation

**Even parity**: Probability density |ψ(x)|² unchanged under reflection
**Odd parity**: Probability density still even (|−ψ|² = |ψ|²), but phase flips

## Application to Harmonic Oscillator

From [[First Three Hermite Polynomials]]:
- |0⟩: H₀ = 1 (even) → ψ₀ even
- |1⟩: H₁ = y (odd) → ψ₁ odd  
- |2⟩: H₂ = 1-2y² (even) → ψ₂ even

**General**: |n⟩ has parity (-1)ⁿ

## Related
- Next: [[Parity-Hamiltonian Commutation]]
- General concept: [[Even and Odd Functions]]
- Used in: [[Week 11.2 - Position Space Solution and Parity]]