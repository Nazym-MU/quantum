Component of momentum operator in the radial direction.
## Position Space Form
$$\bra{r}\,\hat p_r\,\ket{\psi} = -i\hbar\left( \frac{\partial}{\partial r} + \frac{1}{r} \right)\bra{r}\psi\rangle$$
Or as an operator:
$$\hat p_r = -i\hbar\left( \frac{\partial}{\partial r} + \frac{1}{r} \right)$$
Alternative Form
$$\hat p_r = -i\hbar\,\frac{1}{r}\frac{\partial}{\partial r}r$$
This form makes hermiticity more apparent.
## Radial Kinetic Energy
The radial part of kinetic energy is:
$$\bra{r}\,\frac{\hat p_r^{\,2}}{2\mu}\,\ket{\psi}
= -\frac{\hbar^2}{2\mu}\left( \frac{\partial^2}{\partial r^2}
+ \frac{2}{r}\frac{\partial}{\partial r} \right)\bra{r}\psi\rangle$$
## Why Not Just $-i\hbar\,\partial/\partial r$?
The additional $1/r$ term ensures $\hat p_r$ is Hermitian.   In spherical coordinates, the volume element is $d^3r = r^2 \sin\theta\, dr\, d\theta\, d\phi$.  The factor $r^2$ affects the hermiticity requirement.
For an operator to be Hermitian:
$$\int \psi_1^*\,\hat p_r\,\psi_2 \, d^3r
= \int (\hat p_r \psi_1)^*\,\psi_2 \, d^3r$$
The form $\hat p_r = -i\hbar\left( \frac{\partial}{\partial r} + \frac{1}{r} \right)$ satisfies this with the $r^2$ volume element.
## Connection to Classical Radial Momentum
Classically: $p_r = m\frac{dr}{dt} = m\dot r$.
## Total Momentum Decomposition
$$\hat p^{\,2} = \hat p_r^{\,2} + \frac{\hat L^{\,2}}{r^2}$$
This separates momentum into radial and angular parts, which appears in the Hamiltonian as radial kinetic energy plus rotational kinetic energy.
Related: [[Radial Schrödinger Equation]], [[Radial Kinetic Energy Decomposition]]
