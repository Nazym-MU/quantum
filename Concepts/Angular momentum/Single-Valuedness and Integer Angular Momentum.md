Why orbital angular momentum quantum number $l$ must be an integer.
## The Differential Equation
From $\hat{L}_z |l, m\rangle = m\hbar |l, m\rangle$ in position space:
$$-i\hbar\frac{\partial}{\partial \phi}\langle \theta, \phi | l, m \rangle = m\hbar \langle \theta, \phi | l, m \rangle$$
Solution: $\langle \theta, \phi | l, m \rangle \propto e^{im\phi}$
## Single-Valuedness Requirement
Wave functions must be **single-valued**: approaching angle $\phi$ from different directions must give the same value.
$$\psi(\phi) = \psi(\phi + 2\pi)$$
This is necessary for:
1. Derivatives to be well-defined
2. $\hat{L}_z$ to be Hermitian (ensures unitarity of rotations)
3. Probability to be conserved under rotations
## Consequence for m
From $e^{im\phi} = e^{im(\phi + 2\pi)}$:
$$e^{im\phi} = e^{im\phi} e^{2\pi i m}$$

This requires $e^{2\pi i m} = 1$, which means:
$$m = 0, \pm 1, \pm 2, \pm 3, \ldots$$
**m must be an integer.**
## Consequence for l
From Chapter 3, we know $m$ ranges from $-l$ to $+l$ in integer steps. If $m$ is always integer, then:
$$l = 0, 1, 2, 3, \ldots$$
## Why Spin is Different
Intrinsic spin angular momentum (like electron spin-1/2) does NOT arise from literal rotation in position space. Spin operators cannot be represented as differential operators in coordinate space, so the single-valuedness argument doesn't apply.
This is why spin can have half-integer values ($s = 1/2, 3/2, \ldots$) but orbital angular momentum cannot.
## Physical Interpretation
If an electron were literally spinning about an axis, that would be orbital motion and $l$ would be integer. Since electron spin has $s = 1/2$, we know it's fundamentally different - it's intrinsic angular momentum, not rotational motion.

Related: [[Position-Space Representation of Orbital Angular Momentum]], [[Orbital Angular Momentum as Generator of Rotations]]
