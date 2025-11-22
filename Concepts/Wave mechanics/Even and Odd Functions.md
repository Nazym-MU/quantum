Functions classified by their symmetry under reflection f(x) → f(-x).
## Even Functions
Symmetric under reflection:
$$f(-x) = f(x)$$
**Examples**:
- Polynomials: 1, x², x⁴, x⁶, ...
- Trigonometric: cos(x), sec(x)
- Exponential: e^(-x²), cosh(x)
- Absolute value: |x|
**Graph**: Symmetric about y-axis

**Property**: ∫₋ₐᵃ f(x)dx = 2∫₀ᵃ f(x)dx (can integrate over half domain and double)
## Odd Functions
Antisymmetric under reflection:
$$f(-x) = -f(x)$$

**Examples**:
- Polynomials: x, x³, x⁵, x⁷, ...
- Trigonometric: sin(x), tan(x)
- Exponential: sinh(x)
- Linear combinations: x·e^(-x²)
**Graph**: Rotationally symmetric about origin (180° rotation)
**Property**: ∫₋ₐᵃ f(x)dx = 0 (contributions from ±x cancel)
## Mixed Functions
Most functions are neither even nor odd:
- eˣ
- x² + x
- cos(x) + sin(x)
**Decomposition**: Any function can be written as sum of even and odd parts:
$$f(x) = f_{\text{even}}(x) + f_{\text{odd}}(x)$$

where:
$$f_{\text{even}}(x) = \frac{f(x) + f(-x)}{2}$$
$$f_{\text{odd}}(x) = \frac{f(x) - f(-x)}{2}$$
## Quantum Mechanical Connection
Functions correspond to [[Parity Operator]] eigenstates:
- Even functions: eigenvalue +1
- Odd functions: eigenvalue -1
For [[Harmonic Oscillator]]:
- Energy eigenstate |n⟩ has parity (-1)ⁿ
- [[Hermite Polynomials]] Hₙ are even/odd based on n

## Operations Preserving Symmetry

**Products**:
- even × even = even
- odd × odd = even  
- even × odd = odd

**Derivatives**:
- d(even)/dx = odd
- d(odd)/dx = even

**Powers**:
- (even)ⁿ = even for any n
- (odd)ⁿ = odd if n odd, even if n even

## Physical Applications

Potentials with even symmetry V(-x) = V(x):
- Allow energy eigenstates with definite parity
- Simplify solving Schrödinger equation
- Examples: harmonic oscillator, infinite square well (centered)

## Related
- [[Parity Operator]]
- [[Hermite Polynomials]]
- [[Parity Operator Action]]
- [[Parity-Hamiltonian Commutation]]