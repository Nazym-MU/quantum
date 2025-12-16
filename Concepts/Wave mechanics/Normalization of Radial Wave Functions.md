$$\psi(r,\theta,\phi) = R_{nl}(r)Y_{lm}(\theta,\phi)$$
$$\int_0^\infty \int_0^\pi \int_0^{2\pi} |\psi|^2 r^2 \sin\theta \, dr \, d\theta \, d\phi = 1$$
Since spherical harmonics are already normalized:

$$\int_0^{2\pi} d\phi \int_0^\pi \sin\theta \, d\theta \, |Y_{lm}|^2 = 1$$
The radial part normalizes separately:
$$\int_0^\infty r^2 |R_{nl}(r)|^2 dr = 1$$
## In Terms of u(r)
Using $u(r) = rR(r)$:
$$\int_0^\infty |u_{nl}(r)|^2 dr = 1$$
This is simpler because the $r^2$ factor is absorbed into $u$.
## Bound States vs Continuum
**Bound states** ($E < 0$): Wave functions decay exponentially at large $r$ → normalizable with this condition
**Continuum states** ($E > 0$): Wave functions oscillate at large $r$ → use Dirac delta normalization instead
## Example: Ground State of Hydrogen
$$R_{1,0}(r) = 2\left(\frac{Z}{a_0}\right)^{3/2}e^{-Zr/a_0}$$
Check normalization:
$$\int_0^\infty r^2 |R_{1,0}|^2 dr = 4\left(\frac{Z}{a_0}\right)^3 \int_0^\infty r^2 e^{-2Zr/a_0} dr$$
Using $\int_0^\infty x^2 e^{-ax} dx = 2/a^3$:
$$= 4\left(\frac{Z}{a_0}\right)^3 \cdot \frac{2}{(2Z/a_0)^3} = 4\left(\frac{Z}{a_0}\right)^3 \cdot \frac{a_0^3}{4Z^3} = 1$$

Related: [[Radial Schrödinger Equation]], [[Hydrogen Wave Functions]], [[Normalization of Spherical Harmonics]]
