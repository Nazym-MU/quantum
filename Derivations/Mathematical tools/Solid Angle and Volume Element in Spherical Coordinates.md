Derivation of the volume element $d^3r = r^2 dr \, d\Omega$ and solid angle $d\Omega = \sin\theta \, d\theta \, d\phi$.
## Volume Element in Spherical Coordinates
A small volume element at position $(r, \theta, \phi)$ has dimensions:
- Radial extent: $dr$
- Arc length in $\theta$ direction: $r \, d\theta$
- Arc length in $\phi$ direction: $r\sin\theta \, d\phi$
Volume:
$$d^3r = dr \times (r \, d\theta) \times (r\sin\theta \, d\phi) = r^2 \sin\theta \, dr \, d\theta \, d\phi$$
**Solid angle** is the 3D analog of ordinary angle in 2D.
**2D angle** (in radians): arc length divided by radius
$$d\phi_{\text{2D}} = \frac{ds}{r}$$
**3D solid angle**: surface area divided by radius squared
$$d\Omega = \frac{dS}{r^2}$$
## Surface Element
$$dS = (r \, d\theta)(r\sin\theta \, d\phi) = r^2 \sin\theta \, d\theta \, d\phi$$
$$d\Omega = \frac{dS}{r^2} = \sin\theta \, d\theta \, d\phi$$
$$d^3r = r^2 dr \, d\Omega$$
## Total Solid Angle
Integrating over all directions:

$$\int_{4\pi} d\Omega = \int_0^{2\pi} d\phi \int_0^\pi \sin\theta \, d\theta$$

$$= 2\pi \int_0^\pi \sin\theta \, d\theta = 2\pi[-\cos\theta]_0^\pi = 2\pi(1 - (-1)) = 4\pi$$
The total solid angle subtended by a sphere (or any closed surface) is $4\pi$ steradians.
## Probability
For normalized wave function $\psi(r, \theta, \phi)$:

$$\int_0^\infty \int_{4\pi} |\psi(r, \theta, \phi)|^2 r^2 dr \, d\Omega = 1$$
- $|\psi|^2 r^2 dr \, d\Omega$ = probability in volume element
- $|\psi|^2 r^2 dr$ = radial probability density
- $|\psi|^2 d\Omega$ = angular probability density (if integrated over $r$)
Related: [[Normalization of Spherical Harmonics]], [[Probability Interpretation of Spherical Harmonics]]
