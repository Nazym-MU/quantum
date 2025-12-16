For $m \geq 0$:
$$Y_{l,m}(\theta, \phi) = (-1)^l \sqrt{\frac{2l+1}{4\pi}\frac{(l+m)!}{(l-m)!}} e^{im\phi} \frac{1}{\sin^m\theta} \frac{d^{l-m}}{d(\cos\theta)^{l-m}} \sin^{2l}\theta$$
For $m < 0$:

$$Y_{l,m}(\theta, \phi) = (-1)^m Y_{l,-m}^*(\theta, \phi)$$
## Connection to Legendre Polynomials
For $m = 0$:

$$Y_{l,0}(\theta, \phi) = \sqrt{\frac{2l+1}{4\pi}} P_l(\cos\theta)$$
where $P_l(x)$ is the Legendre polynomial of degree $l$.
## Explicit Forms for l = 0, 1, 2

**l = 0 (s orbital)**:
$$Y_{0,0} = \frac{1}{\sqrt{4\pi}}$$

**l = 1 (p orbitals)**:
$$Y_{1,0} = \sqrt{\frac{3}{4\pi}} \cos\theta$$

$$Y_{1,\pm 1} = \mp\sqrt{\frac{3}{8\pi}} \sin\theta \, e^{\pm i\phi}$$

**l = 2 (d orbitals)**:
$$Y_{2,0} = \sqrt{\frac{5}{16\pi}} (3\cos^2\theta - 1)$$

$$Y_{2,\pm 1} = \mp\sqrt{\frac{15}{8\pi}} \sin\theta \cos\theta \, e^{\pm i\phi}$$

$$Y_{2,\pm 2} = \sqrt{\frac{15}{32\pi}} \sin^2\theta \, e^{\pm 2i\phi}$$
The phase factor $(-1)^l$ ensures $Y_{l,0}(\theta, \phi)$ is real and positive at $\theta = 0$.
## Symmetry Properties
- **Real part**: Has $\cos(m\phi)$ dependence
- **Imaginary part**: Has $\sin(m\phi)$ dependence
- **$\theta$ dependence**: Polynomial in $\cos\theta$ and $\sin\theta$

Related: [[Cartesian Forms of Spherical Harmonics]], [[Spherical Harmonics Definition]], [[Deriving spherical harmonics using ladder operators]]
