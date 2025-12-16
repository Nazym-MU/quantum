## Volume Element in Spherical Coordinates

$$d^3r = r^2 dr \sin\theta d\theta d\phi = r^2 dr \, d\Omega$$
where the solid angle element is:
$$d\Omega = \sin\theta \, d\theta \, d\phi$$
[[Solid Angle and Volume Element in Spherical Coordinates]].
## Total Wave Function Normalization
For complete wave function $\psi(r, \theta, \phi) = R(r) Y_{l,m}(\theta, \phi)$:
$$\int_0^\infty \int_0^\pi \int_0^{2\pi} |\psi(r, \theta, \phi)|^2 r^2 dr \sin\theta d\theta d\phi = 1$$
## Separate Normalization
We can normalize radial and angular parts separately:
**Radial normalization**:
$$\int_0^\infty r^2 |R(r)|^2 dr = 1$$
**Angular normalization**:
$$\int_0^{2\pi} d\phi \int_0^\pi \sin\theta d\theta \, |Y_{l,m}(\theta, \phi)|^2 = 1$$
Or more compactly:
$$\int_{4\pi} d\Omega \, |Y_{l,m}(\theta, \phi)|^2 = 1$$
## Total Solid Angle

The integral over all directions:

$$\int_{4\pi} d\Omega = \int_0^{2\pi} d\phi \int_0^\pi \sin\theta d\theta = 4\pi$$

This is analogous to the full angle around a circle being $2\pi$ radians.
## Orthonormality
Different spherical harmonics are orthogonal:
$$\int_{4\pi} d\Omega \, Y_{l',m'}^*(\theta, \phi) Y_{l,m}(\theta, \phi) = \delta_{l,l'} \delta_{m,m'}$$

This allows us to expand any function on the sphere in terms of spherical harmonics.
Related: [[Spherical Harmonics Definition]], [[Solid Angle and Volume Element in Spherical Coordinates]], [[Probability Interpretation of Spherical Harmonics]]
