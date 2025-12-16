Derivation of quantized energy levels $E_n = -\frac{13.6 \text{ eV}}{n^2}$ for hydrogen.
## Radial Equation
For Coulomb potential $V(r) = -Ze^2/r$:
$$-\frac{\hbar^2}{2\mu}\frac{d^2u}{dr^2} + \left[\frac{l(l+1)\hbar^2}{2\mu r^2} - \frac{Ze^2}{r}\right]u = Eu$$
## Dimensionless Variables
For bound states $E < 0$, define $E = -|E|$
Introduce:
$$\rho = \sqrt{\frac{8\mu|E|}{\hbar^2}} \, r$$
Then equation becomes:
$$\frac{d^2u}{d\rho^2} = \left[1 - \frac{\lambda}{\rho} + \frac{l(l+1)}{\rho^2}\right]u$$
where:
$$\lambda = \frac{Ze^2}{\hbar}\sqrt{\frac{\mu}{2|E|}}$$
## Asymptotic Behavior
**Large $\rho$**: equation reduces to $\frac{d^2u}{d\rho^2} \approx u$
Solutions: $u \sim e^{\pm \rho}$
Discard $e^{+\rho}$ (not normalizable), keep $e^{-\rho}$
**Small $\rho$**: From previous analysis, $u \sim \rho^{l+1}$
## Ansatz

Try:
$$u(\rho) = \rho^{l+1}e^{-\rho}F(\rho)$$

where $F(\rho)$ is a polynomial to be determined.

## Differential Equation for F

Substituting into radial equation:

$$\frac{d^2F}{d\rho^2} + \left(\frac{2l+2}{\rho} - 1\right)\frac{dF}{d\rho} + \left(\frac{\lambda - l - 1}{\rho}\right)F = 0$$

## Power Series Solution

Try $F(\rho) = \sum_{k=0}^\infty c_k \rho^k$

Recursion relation:
$$\frac{c_{k+1}}{c_k} = \frac{k + l + 1 - \lambda}{(k+1)(k+2l+2)}$$

## Series Termination Requirement

For large $k$:
$$\frac{c_{k+1}}{c_k} \to \frac{1}{k}$$

This is the recursion for $e^\rho$, which would give $u \sim e^{\rho/2}$ (not normalizable!)

**Must terminate series**: Set $\lambda = n_r + l + 1$ where $n_r = 0, 1, 2, \ldots$

Define **principal quantum number**: $n = n_r + l + 1 = 1, 2, 3, \ldots$

## Energy Quantization

From $\lambda = \frac{Ze^2}{\hbar}\sqrt{\frac{\mu}{2|E|}} = n$:

$$\frac{Ze^2}{\hbar}\sqrt{\frac{\mu}{2|E|}} = n$$

Solving for $E$:
$$|E| = \frac{\mu Z^2 e^4}{2\hbar^2 n^2}$$

Therefore:
$$\boxed{E_n = -\frac{\mu Z^2 e^4}{2\hbar^2 n^2}}$$

## In Terms of Fine-Structure Constant

Using $\alpha = e^2/\hbar c$:

$$E_n = -\frac{\mu c^2 Z^2 \alpha^2}{2n^2}$$

For hydrogen ($Z=1$, $\mu \approx m_e$):

$$\boxed{E_n = -\frac{13.6 \text{ eV}}{n^2}}$$

## Quantum Number Constraints

From $n = n_r + l + 1$:
- $n_r = 0, 1, 2, \ldots$
- $l = 0, 1, 2, \ldots, n-1$
- For each $l$: $m = -l, \ldots, l$

Related: [[Energy Levels of Hydrogen Atom]], [[Hydrogenic Atom Hamiltonian]], [[Fine-Structure Constant]]
