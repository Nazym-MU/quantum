Derivation of position-space representation $\hat{L}_z \rightarrow -i\hbar\frac{\partial}{\partial\phi}$.
## Starting Point
Rotation about z-axis by angle $d\phi$:

$$\hat{R}(d\phi\hat{k})|r, \theta, \phi\rangle = |r, \theta, \phi + d\phi\rangle$$
$$\langle r, \theta, \phi|\hat{R}(d\phi\hat{k}) = \langle r, \theta, \phi - d\phi|$$
Action on state:
$$\langle r, \theta, \phi|\hat{R}(d\phi\hat{k})|\psi\rangle = \langle r, \theta, \phi - d\phi|\psi\rangle$$
## Taylor Expansion
Expand in small $d\phi$:
$$\langle r, \theta, \phi - d\phi|\psi\rangle = \langle r, \theta, \phi|\psi\rangle - d\phi \frac{\partial}{\partial\phi}\langle r, \theta, \phi|\psi\rangle$$
## Generator Form
The rotation operator:
$$\hat{R}(d\phi\hat{k}) = 1 - \frac{i}{\hbar}\hat{L}_z d\phi$$
Therefore:
$$\langle r, \theta, \phi|\left(1 - \frac{i}{\hbar}\hat{L}_z d\phi\right)|\psi\rangle = \langle r, \theta, \phi|\psi\rangle - d\phi \frac{\partial}{\partial\phi}\langle r, \theta, \phi|\psi\rangle$$
$$\langle r, \theta, \phi|\psi\rangle - d\phi\frac{i}{\hbar}\langle r, \theta, \phi|\hat{L}_z|\psi\rangle = \langle r, \theta, \phi|\psi\rangle - d\phi \frac{\partial}{\partial\phi}\langle r, \theta, \phi|\psi\rangle$$
$$\frac{i}{\hbar}\langle r, \theta, \phi|\hat{L}_z|\psi\rangle = \frac{\partial}{\partial\phi}\langle r, \theta, \phi|\psi\rangle$$
## Result
Comparing both sides:
$$\langle r, \theta, \phi|\hat{L}_z|\psi\rangle = -i\hbar\frac{\partial}{\partial\phi}\langle r, \theta, \phi|\psi\rangle$$
Thus in position space:
$$\boxed{\hat{L}_z \rightarrow -i\hbar\frac{\partial}{\partial\phi}}$$
This is exactly analogous to:
$$\hat{p}_x \rightarrow -i\hbar\frac{\partial}{\partial x}$$
Linear momentum generates translations; angular momentum generates rotations. Both become derivative operators in position space.

Related: [[Position-Space Representation of Orbital Angular Momentum]], [[Single-Valuedness and Integer Angular Momentum]]
