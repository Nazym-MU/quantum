## Position-Space Density Matrix
For a density operator ρ̂, the position-space representation is:
$$\rho(x, x') = \langle x|\hat{\rho}|x'\rangle$$

## Diagonal Elements: Classical Probability
$$\rho(x, x) = \langle x|\hat{\rho}|x\rangle = P(x)$$

This is the probability density at position x (like |ψ(x)|² for pure states).

## Off-Diagonal Elements: Quantum Coherence
$$\rho(x, x') \text{ for } x \neq x'$$

Encode quantum interference and phase relationships between different positions.

## Pure State Example
For |ψ⟩: ρ̂ = |ψ⟩⟨ψ|
$$\rho(x, x') = \langle x|\psi\rangle\langle\psi|x'\rangle = \psi(x)\psi^*(x')$$

Diagonal: ρ(x,x) = |ψ(x)|²

## Mixed State Example
Classical mixture: 50% at x=a, 50% at x=b
$$\hat{\rho} = \frac{1}{2}|a\rangle\langle a| + \frac{1}{2}|b\rangle\langle b|$$
$$\rho(x,x') = \frac{1}{2}[\delta(x-a)\delta(x'-a) + \delta(x-b)\delta(x'-b)]$$

No off-diagonal coherence between x=a and x=b.

## Expectation Values
$$\langle \hat{A}\rangle = \text{Tr}(\hat{\rho}\hat{A}) = \int dx \, \langle x|\hat{\rho}\hat{A}|x\rangle$$

For position:
$$\langle x\rangle = \int dx \, x\rho(x,x)$$

## Key Distinction
- **Pure state superposition** (ψ₁ + ψ₂)/√2: Has off-diagonal terms → quantum interference
- **Mixed state** p₁|ψ₁⟩⟨ψ₁| + p₂|ψ₂⟩⟨ψ₂|: No off-diagonal terms between ψ₁ and ψ₂ → classical mixture