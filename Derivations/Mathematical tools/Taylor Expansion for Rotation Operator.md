To rotate by finite angle φ, apply many infinitesimal rotations:
$$d\phi = \lim_{N \to \infty} \frac{\phi}{N}$$
Composition of N infinitesimal rotations:
$$\hat{R}(\phi\hat{k}) = \lim_{N\to\infty} \left[\hat{R}(d\phi\hat{k})\right]^N = \lim_{N\to\infty} \left[1 - \frac{i}{\hbar}\hat{J}_z\frac{\phi}{N}\right]^N$$
## Exponential Form
$$\lim_{N\to\infty}\left(1 + \frac{x}{N}\right)^N = e^x$$
We get:
$$\hat{R}(\phi\hat{k}) = e^{-i\hat{J}_z\phi/\hbar}$$
## Taylor Series
Expanding the exponential:
$$e^{-i\hat{J}_z\phi/\hbar} = 1 - \frac{i\phi}{\hbar}\hat{J}_z + \frac{1}{2!}\left(\frac{-i\phi}{\hbar}\right)^2\hat{J}_z^2 + \frac{1}{3!}\left(\frac{-i\phi}{\hbar}\right)^3\hat{J}_z^3 + \cdots$$
For small φ, keep only first-order term:
$$\hat{R}(d\phi\hat{k}) \approx 1 - \frac{i}{\hbar}\hat{J}_z d\phi$$
## Action on Eigenstates
For eigenstate $\hat{J}_z|+z\rangle = \frac{\hbar}{2}|+z\rangle$:
$$\hat{J}_z^n|+z\rangle = \left(\frac{\hbar}{2}\right)^n|+z\rangle$$
Substituting into Taylor series:
$$\hat{R}(\phi\hat{k})|+z\rangle = \left[1 - \frac{i\phi}{2} + \frac{1}{2!}\left(\frac{-i\phi}{2}\right)^2 + \cdots\right]|+z\rangle = e^{-i\phi/2}|+z\rangle$$
**Result**: Only picks up phase factor (no change in state direction).
## General Axis
For rotation about arbitrary axis n̂: $$\hat{R}(\theta\hat{n}) = e^{-i(\hat{\vec{J}} \cdot \hat{n})\theta/\hbar}$$
where $\hat{\vec{J}} \cdot \hat{n} = J_x n_x + J_y n_y + J_z n_z$
## Related
- [[Rotation Operators]]
- [[Rotation Operator from Infinitesimal]]