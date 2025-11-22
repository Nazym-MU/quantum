## Recursion Relation with ε = 2n + 1
From [[Series Termination and Energy Quantization]], using ε = 2n + 1:
$$a_{k+2} = \frac{2k + 1 - (2n+1)}{(k+2)(k+1)} a_k = \frac{2(k-n)}{(k+2)(k+1)} a_k$$
## n = 0: Ground State
ε = 2(0) + 1 = 1
**Check a₂**:
$$a_2 = \frac{2(0-0)}{2 \cdot 1} a_0 = 0$$
Series terminates immediately. Must set a₁ = 0 (otherwise odd series continues).
**Result**: h₀(y) = a₀
**Convention**: Set a₀ = 1
$$H_0(y) = 1$$
**Verification in Eq. 7.44**:
$$\langle x|0\rangle = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} \exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$
No polynomial factor (just the Gaussian), consistent with H₀ = 1 ✓
## n = 1: First Excited State
ε = 2(1) + 1 = 3
**Check a₃**:
$$a_3 = \frac{2(1-1)}{3 \cdot 2} a_1 = 0$$
Series terminates after first term. Must set a₀ = 0 (even series doesn't terminate).
**Result**: h₁(y) = a₁y
**Convention**: Set a₁ = 1
$$H_1(y) = y$$
**Verification in Eq. 7.46**:
$$\langle x|1\rangle = \left(\frac{4m^3\omega^3}{\pi\hbar^3}\right)^{1/4} x \exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$
Polynomial factor is x, and x = √(ℏ/mω) y, so polynomial is proportional to y ✓
## n = 2: Second Excited State
ε = 2(2) + 1 = 5
**Calculate a₂**:
$$a_2 = \frac{2(0-2)}{2 \cdot 1} a_0 = \frac{-4}{2} a_0 = -2a_0$$
**Check a₄**:
$$a_4 = \frac{2(2-2)}{4 \cdot 3} a_2 = 0$$
Series terminates. Must set a₁ = 0.
**Result**: h₂(y) = a₀ + a₂y² = a₀ - 2a₀y² = a₀(1 - 2y²)
**Convention**: Set a₀ = 1
$$H_2(y) = 1 - 2y^2$$
(Or 2y² - 1 in some conventions)
**Verification in Eq. 7.47**:
$$\langle x|2\rangle = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} \frac{1}{\sqrt{2}}\left(\frac{2m\omega x^2}{\hbar} - 1\right) \exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$
Polynomial factor: (2mωx²/ℏ - 1)
Since y² = (mω/ℏ)x², we have mωx²/ℏ = y², so:
2mωx²/ℏ - 1 = 2y² - 1 = -(1 - 2y²)

Consistent up to overall sign/normalization ✓

## Pattern

| n | ε | Polynomial | Parity |
|---|---|------------|--------|
| 0 | 1 | 1 | even |
| 1 | 3 | y | odd |
| 2 | 5 | 1-2y² | even |
| 3 | 7 | y-⅔y³ | odd |

**General properties**:
- Degree of Hₙ is n
- Hₙ has n zeros (nodes)
- Even n → even function
- Odd n → odd function

## Related
- Recursion: [[Power Series Recursion Relation for Hermite Polynomials]]
- Energy quantization: [[Series Termination and Energy Quantization]]
- General properties: [[Hermite Polynomial Properties]]
- Used in: [[Week 11.2 - Position Space Solution and Parity]]