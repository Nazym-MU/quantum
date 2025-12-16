The Laplacian operator $\nabla^2$ in spherical coordinates:
$$\nabla^2 = \frac{\partial^2}{\partial r^2} + \frac{2}{r}\frac{\partial}{\partial r} + \frac{1}{r^2}\left[\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial}{\partial\theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2}{\partial\phi^2}\right]$$
## Connection to L²
The angular part (terms in square brackets) is exactly:
$$\frac{1}{r^2}\left[\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial}{\partial\theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2}{\partial\phi^2}\right] = -\frac{\hat{L}^2}{\hbar^2 r^2}$$
## Position-Space Schrödinger Equation
Using this identification:
$$\left[-\frac{\hbar^2}{2\mu}\nabla^2 + V(r)\right]\langle r|\psi\rangle = E\langle r|\psi\rangle$$
becomes:
$$\left[-\frac{\hbar^2}{2\mu}\left(\frac{\partial^2}{\partial r^2} + \frac{2}{r}\frac{\partial}{\partial r}\right) + \frac{\hat{L}^2}{2\mu r^2} + V(r)\right]\langle r|\psi\rangle = E\langle r|\psi\rangle$$
This matches the radial equation derived in Chapter 9.6, confirming our identification of $\hat{L}^2$ with the angular part of the Laplacian.
## Physical Interpretation
The Laplacian separates naturally into:
- **Radial part**: $\frac{\partial^2}{\partial r^2} + \frac{2}{r}\frac{\partial}{\partial r}$ (motion toward/away from origin)
- **Angular part**: $-\frac{\hat{L}^2}{\hbar^2 r^2}$ (rotational motion)
This separation reflects the split between radial kinetic energy and rotational kinetic energy.
Related: [[Position-Space Representation of Orbital Angular Momentum]], [[Radial Kinetic Energy Decomposition]]
