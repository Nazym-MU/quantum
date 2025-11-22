Any potential near equilibrium approximates V(x) ≈ ½kx².
## Core Concepts
- [[Harmonic Oscillator]] - physical setup and significance
- [[Ladder Operators]] - raising and lowering operators
- [[Number Operator]] - counts energy quanta
- [[Zero-Point Energy]] - ground state has E₀ = ½ℏω
## Key Equations
**Hamiltonian:**
$$\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2 = \hbar\omega\left(\hat{N} + \frac{1}{2}\right)$$
→ Derivation: [[Hamiltonian in Terms of Number Operator]]
**Energy eigenvalues:**
$$E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0,1,2,\ldots$$
→ Derivation: [[Number Operator Eigenvalue Derivation]]
**Ladder operator commutator:**
$$[\hat{a}, \hat{a}^\dagger] = 1$$
→ Derivation: [[Ladder Operator Commutation Relation]]
**Ladder operator actions:**
$$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$$
$$\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$$
→ Derivations: [[Raising Operator Matrix Elements]], [[Lowering Operator Matrix Elements]]
**Excited state generation:**
$$|n\rangle = \frac{(\hat{a}^\dagger)^n}{\sqrt{n!}}|0\rangle$$
→ Derivation: [[Excited State Generation]]
## Wave Functions
**Ground state:**
$$\langle x|0\rangle = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-m\omega x^2/2\hbar}$$
→ Derivation: [[Ground State Wave Function Derivation]]
**Excited states:**
Applied by position-space ladder operator $(x - \frac{\hbar}{m\omega}\frac{d}{dx})^n$
→ Derivation: [[Harmonic Oscillator Excited State Wave Functions]]
**Full structure:**
- [[Harmonic Oscillator Wave Functions]]
- [[Hermite Polynomials]]
- [[Node Structure in Energy Eigenstates]]
- [[Classical Turning Points]]
## Uncertainties
**Position uncertainty:**
$$\langle\Delta x^2\rangle_n = \frac{\hbar}{2m\omega}(2n+1)$$
→ Derivation: [[Harmonic Oscillator Position Uncertainty]]
**Momentum uncertainty:**
$$\langle\Delta p^2\rangle_n = \frac{m\hbar\omega}{2}(2n+1)$$
→ Derivation: [[Harmonic Oscillator Momentum Uncertainty]]
**Ground state:** ΔxΔp = ℏ/2 (minimum uncertainty)
→ Explanation: [[Zero-Point Energy Physical Origin]]
## Position-Space Solution Method
Alternative approach solving the Schrödinger equation directly:
- [[Position-Space Harmonic Oscillator Solution]]
- Reveals [[Hermite Polynomials]] structure
- Shows [[Parity Operator]] symmetry
- [[Series Termination and Energy Quantization]]
## Matrix Representations
- [[Raising Operator Matrix Representation]]
- [[Lowering Operator Matrix Representation]]
- [[Why Ladder Operators Are Not Diagonal]]
- [[Why Position and Momentum Averages Vanish in Energy Eigenstates]]