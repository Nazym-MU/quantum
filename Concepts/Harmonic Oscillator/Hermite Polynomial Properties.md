Properties of [[Hermite Polynomials]] Hₙ(y) that appear in [[Harmonic Oscillator]] wave functions.

## Basic Properties

**Degree**: Hₙ(y) is polynomial of degree n

**Leading coefficient**: Highest power term is 2ⁿyⁿ

**Parity**: 
$$H_n(-y) = (-1)^n H_n(y)$$
- Even n: even polynomial
- Odd n: odd polynomial

Derivation: [[First Three Hermite Polynomials]]

## Zeros (Nodes)

Hₙ(y) has exactly **n distinct real zeros**, all located in interval where classical motion is allowed.

**Connection to quantum mechanics**: 
- |n⟩ energy eigenstate has n nodes in ψₙ(x)
- Higher energy → more oscillations → more nodes

See: [[Node Structure in Energy Eigenstates]]

## Recursion Relations

**Three-term recursion**:
$$H_{n+1}(y) = 2yH_n(y) - 2nH_{n-1}(y)$$

Starting from H₀ = 1, H₁ = 2y, can generate all higher polynomials.

**Derivative relation**:
$$\frac{dH_n}{dy} = 2nH_{n-1}(y)$$

## Differential Equation

Hermite polynomials satisfy:
$$\frac{d^2H_n}{dy^2} - 2y\frac{dH_n}{dy} + 2nH_n = 0$$

This emerges from [[Differential Equation for h(y)]] with ε = 2n + 1.

## Orthogonality

With weight function e^(-y²):
$$\int_{-\infty}^{\infty} H_m(y)H_n(y)e^{-y^2}dy = \sqrt{\pi}2^n n! \,\delta_{mn}$$

**Physical meaning**: Different energy eigenstates are orthogonal when integrated with Gaussian weight.

## Generating Function

$$e^{2yt - t^2} = \sum_{n=0}^{\infty} \frac{H_n(y)}{n!}t^n$$

Provides compact way to generate all Hermite polynomials.

## Rodrigues Formula

$$H_n(y) = (-1)^n e^{y^2} \frac{d^n}{dy^n}(e^{-y^2})$$

Alternative definition connecting to Gaussian function.

## Explicit Forms

- H₀(y) = 1
- H₁(y) = 2y
- H₂(y) = 4y² - 2
- H₃(y) = 8y³ - 12y
- H₄(y) = 16y⁴ - 48y² + 12
## Asymptotic Behavior

For large n and y ≈ √(2n):
$$H_n(y) \sim 2^{n/2}n^{n/2}e^{y^2/2}\cos\left(y\sqrt{2n} - \frac{n\pi}{2}\right)$$

Shows oscillatory behavior near classical turning points.

## Physical Interpretation

In harmonic oscillator wave function:
$$\psi_n(x) = N_n H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right) e^{-m\omega x^2/2\hbar}$$

- Hₙ provides polynomial modulation
- e^(-mωx²/2ℏ) provides Gaussian envelope
- Combined: nodes occur where Hₙ = 0
- Probability density vanishes at n locations

## Related
- [[Hermite Polynomials]]
- [[First Three Hermite Polynomials]]
- [[Harmonic Oscillator Wave Functions]]
- [[Node Structure in Energy Eigenstates]]
- [[Even and Odd Functions]]