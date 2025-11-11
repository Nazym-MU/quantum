## Definition
The momentum-space wave function:
$$\tilde{\psi}(p) = \langle p|\psi\rangle$$

Gives the amplitude to find the particle with momentum p.

## Fourier Transform Relation
**Position → Momentum:**
$$\tilde{\psi}(p) = \int dx \, \langle p|x\rangle\langle x|\psi\rangle = \int dx \, \frac{1}{\sqrt{2\pi\hbar}}e^{-ipx/\hbar}\psi(x)$$

**Momentum → Position:**
$$\psi(x) = \int dp \, \langle x|p\rangle\langle p|\psi\rangle = \int dp \, \frac{1}{\sqrt{2\pi\hbar}}e^{ipx/\hbar}\tilde{\psi}(p)$$

## Probability Interpretation
$$P(p)dp = |\tilde{\psi}(p)|^2 dp$$

**Normalization:**
$$\int_{-\infty}^{\infty} |\tilde{\psi}(p)|^2 dp = 1$$

## Expectation Values
**Momentum:**
$$\langle p_x\rangle = \int dp \, p|\tilde{\psi}(p)|^2$$

**Position in momentum space:**
$$\langle x\rangle = \int dp \, \tilde{\psi}^*(p)\left(i\hbar\frac{\partial}{\partial p}\right)\tilde{\psi}(p)$$

## Complementarity
Position and momentum representations are dual:
- Sharp in position → broad in momentum
- Sharp in momentum → broad in position
- Gaussian in position ↔ Gaussian in momentum (minimum uncertainty)