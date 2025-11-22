Alternative method for solving the [[Harmonic Oscillator]] by directly solving the Schrödinger equation in position space.
## Why This Method
**Operator method:** Abstract, uses [[Ladder Operators]]
**Position-space method:** Direct differential equation solution
- Provides explicit wave functions ψ(x)
- Generalizes to 3D problems
- Reveals [[Hermite Polynomials]]
- Demonstrates symmetry analysis
## The Schrödinger Equation
Time-independent equation in position space:
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + \frac{1}{2}m\omega^2x^2\psi = E\psi$$
**Dimensionless form:**
$$\frac{d^2\psi}{dy^2} = (y^2 - \varepsilon)\psi$$
where y = √(mω/ℏ)x and ε = 2E/ℏω
→ Derivation: [[TISE in Dimensionless Variables]]
## Solution Strategy
**Step 1: Asymptotic behavior**
For |y| → ∞: ψ(y) ~ e^(-y²/2)
→ Derivation: [[Asymptotic Solution for Harmonic Oscillator]]
**Step 2: Factor out asymptotic part**
Write ψ(y) = h(y)e^(-y²/2), obtain equation for h(y):
$$\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + (\varepsilon - 1)h = 0$$
→ Derivation: [[Differential Equation for h(y)]]
**Step 3: Power series solution**
Recursion relation:
$$a_{k+2} = \frac{2k + 1 - \varepsilon}{(k+2)(k+1)} a_k$$
→ Derivation: [[Power Series Recursion Relation for Hermite Polynomials]]
**Step 4: Energy quantization**
Series must terminate for normalizability:
$$\varepsilon = 2n + 1 \quad \Rightarrow \quad E_n = \hbar\omega\left(n + \frac{1}{2}\right)$$
→ Derivation: [[Series Termination and Energy Quantization]]
## Hermite Polynomials
The polynomial h(y) = Hₙ(y) where Hₙ is the nth Hermite polynomial.
**First three:**
- H₀(y) = 1
- H₁(y) = y
- H₂(y) = 1 - 2y²
→ Derivation: [[First Three Hermite Polynomials]]
**Properties:**
- [[Hermite Polynomial Properties]]
- [[Hermite Polynomials]]
## Parity Symmetry
**Parity operator:**
$$\hat{\Pi}|x\rangle = |-x\rangle$$
→ Derivation: [[Parity Operator Action]]
**Commutes with Hamiltonian:**
$$[\hat{\Pi}, \hat{H}] = 0$$
→ Derivation: [[Parity-Hamiltonian Commutation]]
**Consequence:** Energy eigenstates have definite parity (-1)ⁿ
- Even n: even functions
- Odd n: odd functions
Related: [[Parity Operator]], [[Even and Odd Functions]]
## Key Results
1. Position-space method confirms operator results
2. Wave functions are Hermite polynomials × Gaussian
3. Parity explains even/odd structure
4. Quantization emerges from normalizability