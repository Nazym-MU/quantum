The [[Harmonic Oscillator]] is central to quantum mechanics because any potential near a minimum approximates V(x) ≈ ½kx² (Taylor expansion). 
### Key Physical Ideas
1. **Universal Approximation**: Near equilibrium, all potentials behave like harmonic oscillators
2. **Operator Solution**: Can solve using ladder operators without wave mechanics
3. **Quantized Energy**: Discrete energy levels En = ℏω(n + ½) with uniform spacing
4. **Zero-Point Energy**: Ground state has E₀ = ½ℏω due to [[Uncertainty|uncertainty principle]]

**Alternative approach**: [[Week 11.2 - Position Space Solution and Parity]] covers solving via Schrödinger equation in position space, revealing [[Hermite Polynomials]] and symmetry properties.
## Essential Formulas
### Hamiltonian and Commutator
- $\hat{H} = \hat{p}^2/2m + \frac{1}{2}mω^2\hat{x}^2$
- \[$\hat{x}, \hat{p_x}$\] = iℏ (see [[Position-Momentum Commutator]])
### Ladder Operators
- $â = \sqrt{(mω/2ℏ)(\hat{x}+ i/mω \hat{p}_x)}$
- $â† = \sqrt{(mω/2ℏ)(x̂ - i/mω p̂_x)}$
- \[â, â†\] = 1 (derivation: [[Ladder Operator Commutation Relation]])
### Number Operator
- $\hat{N} = â^†â$
- $Ĥ = ℏω(\hat{N}+ ½)$
- $\hat{N}|n⟩ = n|n⟩$ (derivation: [[Number Operator Eigenvalue Derivation]])
### Ladder Operator Actions
- $â^†|n⟩ = \sqrt{(n+1)|n+1⟩}$ (derivation: [[Raising Operator Matrix Elements]])
- $â|n⟩ = \sqrt{n|n-1⟩}$ (derivation: [[Lowering Operator Matrix Elements]])
- $|n⟩ = (â†)ⁿ/\sqrt{n!}|0⟩$ (derivation: [[Excited State Generation]])
### Position-Space Wave Functions
- Ground state: $⟨x|0⟩ = (mω/πℏ)^{1/4} e^{-mωx²/2ℏ}$ ([[Ground State Wave Function Derivation]])
- General state: ⟨x|n⟩ obtained by applying ($x̂ - \frac{ℏ}{mω} \frac{d}{dx}$) n times (derivation: [[Harmonic Oscillator Excited State Wave Functions]])
### Uncertainties
- $⟨Δx²⟩ₙ = ℏ/2mω \cdot (2n + 1)$ (derivation: [[Harmonic Oscillator Position Uncertainty]])
- $⟨Δp²⟩ₙ = mℏω/2 \cdot (2n + 1)$ (derivation: [[Harmonic Oscillator Momentum Uncertainty]])
- Ground state: ΔxΔp = ℏ/2 (minimum uncertainty state)
## Conceptual Links
### Core Harmonic Oscillator Concepts
- [[Harmonic Oscillator]]
- [[Ladder Operators]]
- [[Number Operator]]
- [[Zero-Point Energy]]
### Matrix Representations
- [[Raising Operator Matrix Representation]]
- [[Lowering Operator Matrix Representation]]
- Non-diagonal structure explained in [[Why Ladder Operators Are Not Diagonal]]
### Position-Space Properties
- [[Harmonic Oscillator Wave Functions]]
- [[Classical Turning Points]]
- [[Node Structure in Energy Eigenstates]]
- [[Why Position and Momentum Averages Vanish in Energy Eigenstates]]
### Physical Applications
- [[Molecular Vibrations]]
- [[Torsional Oscillations]]
- Connection to quantum field theory (photons as quanta)

## Key Results to Remember

1. Energy eigenvalues: En = ℏω(n + ½), n = 0,1,2,...
2. Equal spacing between levels: ΔE = ℏω
3. Zero-point energy E₀ = ½ℏω arises from \[x̂,p̂\] = iℏ
4. Ground state: minimum uncertainty Gaussian
5. Node count: |n⟩ has n nodes in position space
6. Classical limit: large n → continuous spectrum (ℏω/E → 0)

## Important Derivations

Must be able to rederive:
- [[Ladder Operator Commutation Relation]]
- [[Hamiltonian in Terms of Number Operator]]
- [[Raising Operator Matrix Elements]] (Eq. 7.35)
- [[Lowering Operator Matrix Elements]] (Eq. 7.36)
- [[Excited State Generation]] (Eq. 7.37, Example 7.2)
- [[Ground State Wave Function Derivation]] (Eq. 7.44)
- [[Harmonic Oscillator Excited State Wave Functions]] (Eq. 7.45)
- [[Zero-Point Energy Physical Origin]] (Eqs. 7.50-7.55)