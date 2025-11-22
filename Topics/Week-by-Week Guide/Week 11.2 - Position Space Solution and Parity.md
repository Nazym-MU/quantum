Alternative method for solving the [[Harmonic Oscillator]] by directly solving the Schrödinger equation in position space, revealing [[Hermite Polynomials]] and symmetry properties.
## Why Two Methods?
**Operator method** ([[Week 11 - Harmonic Oscillator]]): Abstract, uses [[Ladder Operators]]
**Position-space method** (this section): Direct differential equation solution
- Provides actual wave functions ψ(x)
- Generalizes to 3D problems (Chapter 10)
- Reveals connection to Hermite polynomials
- Demonstrates power of symmetry analysis
## Position-Space Schrödinger Equation
Time-independent Schrödinger equation in position space:
$$\hat{H}\psi(x) = E\psi(x)$$
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + \frac{1}{2}m\omega^2x^2\psi = E\psi$$
### Dimensionless Form
Introduce dimensionless variable y = √(mω/ℏ) x and ε = 2E/ℏω:
$$\frac{d^2\psi}{dy^2} = (y^2 - \varepsilon)\psi$$
Derivation: [[TISE in Dimensionless Variables]]
**Why nontrivial**: Cannot solve by direct integration (right side contains ψ multiplied by y²-dependent term).
## Solving Strategy
### Step 1: Asymptotic Behavior
For |y| → ∞, neglect ε term:
$$\frac{d^2\psi}{dy^2} \approx y^2\psi$$
Solution: ψ(y) ~ e^(±y²/2)
Derivation: [[Asymptotic Solution for Harmonic Oscillator]]
### Step 2: Factor Out Asymptotic Behavior
Write: $ψ(y) = h(y)e^{-y^2/2}$
This gives differential equation for h(y):
$$\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + (\varepsilon - 1)h = 0$$

Derivation: [[Differential Equation for h(y)]]
### Step 3: Power Series Solution
Assume h(y) = Σ aₖyᵏ, substitute into equation, obtain recursion relation:
$$a_{k+2} = \frac{2k + 1 - \varepsilon}{(k+2)(k+1)} a_k$$
Derivation: [[Power Series Recursion Relation for Hermite Polynomials]]
### Step 4: Termination Condition
**Problem**: Infinite series makes h(y) ~ e^(y²) for large y, giving ψ ~ e^(y²/2) (non-normalizable)
**Solution**: Series must terminate. This requires:
$$\varepsilon = 2n + 1, \quad n = 0,1,2,...$$
Converting back: E = (n + ½)ℏω
Derivation: [[Series Termination and Energy Quantization]]
**Result**: h(y) becomes finite polynomial (Hermite polynomial Hₙ)
## Hermite Polynomials
Polynomials of degree n satisfying the recursion relation with ε = 2n + 1.
**First three**:
- H₀(y) = 1
- H₁(y) = y  
- H₂(y) = 1 - 2y²
Derivation: [[First Three Hermite Polynomials]]
**Properties**:
- Hₙ has degree n
- Even n → even polynomial
- Odd n → odd polynomial
- n nodes (zeros)
See: [[Hermite Polynomial Properties]]
**Wave functions**:
$$\langle x|n\rangle = N_n H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right) \exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$
Matches results from Eqs. 7.44, 7.46, 7.47 (operator method).

## Parity Symmetry

### Parity Operator
Inverts states through origin:
$$\hat{\Pi}|x\rangle = |-x\rangle$$

Action on wave functions:
$$\langle x|\hat{\Pi}|\psi\rangle = \psi(-x)$$

Derivation: [[Parity Operator Action]]

### Eigenvalues
Since Π̂² = 1, eigenvalues are λ = ±1:
$$\psi(-x) = \lambda\psi(x)$$

- λ = +1: even function, ψ(-x) = ψ(x)
- λ = -1: odd function, ψ(-x) = -ψ(x)

### Commutation with Hamiltonian
For harmonic oscillator potential V(x) = ½mω²x² = V(-x):
$$[\hat{\Pi}, \hat{H}] = 0$$

Derivation: [[Parity-Hamiltonian Commutation]]
**Consequence**: Energy eigenstates have definite parity (simultaneous eigenstates).
- |n⟩ has parity (-1)ⁿ
- Even n: even function
- Odd n: odd function

### Power of Symmetry

**Before solving**: Know eigenstates must be even OR odd
**After solving**: Only discover parity by inspecting solutions

This symmetry analysis simplifies solving and reveals structure. Critical for 3D problems.

## Essential Derivations

Must be able to:
1. [[TISE in Dimensionless Variables]] - construct dimensionless form
2. [[Asymptotic Solution for Harmonic Oscillator]] - solve Eq. 7.99
3. [[Differential Equation for h(y)]] - derive Eq. 7.103  
4. [[Power Series Recursion Relation for Hermite Polynomials]] - derive Eq. 7.108
5. [[Series Termination and Energy Quantization]] - explain Eqs. 7.109-7.112, why ε = 2n+1
6. [[First Three Hermite Polynomials]] - Example 7.5, verify Eqs. 7.44, 7.46, 7.47
7. [[Parity Operator Action]] - explain Eqs. 7.118-7.119
8. [[Parity-Hamiltonian Commutation]] - explain Eq. 7.120
## Key Concepts
- [[Hermite Polynomials]]
- [[Parity Operator]]
- [[Even and Odd Functions]]
- [[Normalizability Condition]]
## Summary

Position-space solution:
1. Converts to dimensionless variables
2. Factors out asymptotic behavior e^(-y²/2)
3. Solves for polynomial h(y) via power series
4. Quantization emerges from normalizability requirement
5. Solutions are Hermite polynomials

Parity symmetry:
1. Harmonic oscillator has inversion symmetry V(-x) = V(x)
2. Π̂ commutes with Ĥ
3. Energy eigenstates have definite parity
4. Explains even/odd structure of solutions