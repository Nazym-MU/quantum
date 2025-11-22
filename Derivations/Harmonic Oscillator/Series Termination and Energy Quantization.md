## The Problem: Infinite Series Diverges
From [[Power Series Recursion Relation for Hermite Polynomials]]:
$$a_{k+2} = \frac{2k + 1 - \varepsilon}{(k+2)(k+1)} a_k$$

For large k, this behaves as:
$$\frac{a_{k+2}}{a_k} \approx \frac{2k}{k^2} = \frac{2}{k}$$

## Comparison with e^(y²)

Consider the Taylor series of e^(y²):
$$e^{y^2} = \sum_{n=0}^{\infty} \frac{y^{2n}}{n!} = \sum_{n=0}^{\infty} \frac{1}{n!}y^{2n}$$

Writing as h(y) = Σbₖy^k where only even terms are nonzero:
- b₀ = 1
- b₂ = 1/1! = 1
- b₄ = 1/2! = 1/2
- b₆ = 1/3! = 1/6

**Recursion for bₖ**:
$$\frac{b_{k+2}}{b_k} = \frac{1/(k/2 + 1)!}{1/(k/2)!} = \frac{(k/2)!}{(k/2 + 1)!} = \frac{1}{k/2 + 1}$$

For large k:
$$\frac{b_{k+2}}{b_k} \approx \frac{1}{k/2} = \frac{2}{k}$$

**Same asymptotic behavior as our series!**
If h(y) ~ e^(y²) for large y, then:
$$\psi(y) = h(y)e^{-y^2/2} \sim e^{y^2} \cdot e^{-y^2/2} = e^{y^2/2}$$

This is the **non-normalizable solution** we rejected in [[Asymptotic Solution for Harmonic Oscillator]].

**Normalizability requires**:
$$\int_{-\infty}^{\infty} |\psi(y)|^2 dy < \infty$$

But e^(y²/2) grows exponentially, making this integral diverge.
## The Solution: Series Termination
Make the series terminate (become a finite polynomial).
From recursion relation:
$$a_{k+2} = \frac{2k + 1 - \varepsilon}{(k+2)(k+1)} a_k$$

If numerator vanishes at some k = n:
$$2n + 1 - \varepsilon = 0$$
$$\varepsilon = 2n + 1$$

Then:
- aₙ₊₂ = 0
- aₙ₊₄ = 0 (since it depends on aₙ₊₂)
- All higher terms vanish
**Result**: h(y) is a polynomial of degree n.
## Energy Quantization
Since ε = 2E/ℏω:
$$\frac{2E}{\hbar\omega} = 2n + 1$$
$$E_n = \left(n + \frac{1}{2}\right)\hbar\omega, \quad n = 0,1,2,\ldots$$
This is **quantization**: Only discrete energies give normalizable solutions.

**Same result as operator method** ([[Week 11 - Harmonic Oscillator]]), confirming consistency.
## Even vs Odd Solutions
**If n is even**: Must set a₁ = 0
- Otherwise odd series doesn't terminate
- Get even polynomial
**If n is odd**: Must set a₀ = 0  
- Otherwise even series doesn't terminate
- Get odd polynomial
## Summary
1. Generic solution: Infinite series ~ e^(y²) (bad)
2. Normalizability: Requires series termination
3. Termination: Happens only when ε = 2n + 1
4. Result: Energy quantization + Hermite polynomials

> Normalizability forces physical quantization.

## Related
- Previous: [[Power Series Recursion Relation for Hermite Polynomials]]
- Next: [[First Three Hermite Polynomials]]
- Operator approach: [[Number Operator Eigenvalue Derivation]]
- Used in: [[Week 11.2 - Position Space Solution and Parity]]