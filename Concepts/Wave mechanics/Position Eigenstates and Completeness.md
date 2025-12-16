Position eigenstates |x⟩ satisfy the eigenvalue equation:
$$\hat{x}|x\rangle = x|x\rangle$$
## Key Properties
**Completeness Relation:**
$$\int_{-\infty}^{\infty} dx \, |x\rangle\langle x| = \hat{I}$$

**Orthonormality:**
$$\langle x|x'\rangle = \delta(x-x')$$
The Dirac delta function ensures orthogonality for x ≠ x' and proper normalization.
## Physical Meaning
- |x⟩ represents a particle localized exactly at position x
- Not physically realizable (would require Δx = 0, hence Δp = ∞)
- Mathematical abstraction; physical states are superpositions
## Expressing States
Any state |ψ⟩ can be written as the superposition of position eigenstates:
$$|\psi\rangle = \int dx \, |x\rangle\langle x|\psi\rangle = \int dx \, |x\rangle\psi(x)$$

where $ψ(x) = ⟨x|ψ⟩$ is the wave function.
## Contrast with Discrete States
- Spin: Σᵢ |i⟩⟨i| = Î (discrete sum, δᵢⱼ)
- Position: ∫dx |x⟩⟨x| = Î (continuous integral, δ(x-x'))