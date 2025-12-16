$$\psi_{nlm}(r,\theta,\phi) = R_{nl}(r) Y_{lm}(\theta,\phi)$$
where:
- $n = 1, 2, 3, \ldots$ (principal quantum number)
- $l = 0, 1, \ldots, n-1$ (orbital angular momentum)
- $m = -l, -l+1, \ldots, l$ (magnetic quantum number)
## Ground State (1s)
$$\psi_{100} = R_{1,0}(r) Y_{0,0}(\theta,\phi) = \frac{1}{\sqrt{\pi}}\left(\frac{Z}{a_0}\right)^{3/2}e^{-Zr/a_0}$$
Spherically symmetric ($l=0$, no angular dependence).
## First Excited States (n=2)
**2s state** ($l=0$):
$$R_{2,0} = \frac{1}{2\sqrt{2}}\left(\frac{Z}{a_0}\right)^{3/2}\left(2 - \frac{Zr}{a_0}\right)e^{-Zr/2a_0}$$
Has one radial node.
**2p states** ($l=1$):
$$R_{2,1} = \frac{1}{\sqrt{6}}\left(\frac{Z}{a_0}\right)^{3/2}\frac{Zr}{a_0}e^{-Zr/2a_0}$$
Combined with $Y_{1,m}$ for three degenerate states ($m = -1, 0, 1$).
## Second Excited States (n=3)
**3s state** ($l=0$):
$$R_{3,0} = \frac{1}{9\sqrt{3}}\left(\frac{Z}{a_0}\right)^{3/2}\left(6 - \frac{6Zr}{a_0} + \frac{Z^2r^2}{a_0^2}\right)e^{-Zr/3a_0}$$
Two radial nodes.

**3p states** ($l=1$):
$$R_{3,1} = \frac{1}{9\sqrt{6}}\left(\frac{Z}{a_0}\right)^{3/2}\frac{Zr}{a_0}\left(4 - \frac{2Zr}{3a_0}\right)e^{-Zr/3a_0}$$

One radial node.

**3d states** ($l=2$):
$$R_{3,2} = \frac{1}{9\sqrt{30}}\left(\frac{Z}{a_0}\right)^{3/2}\frac{Z^2r^2}{a_0^2}e^{-Zr/3a_0}$$

No radial nodes.

## Radial Probability Density

Probability of finding electron between $r$ and $r+dr$:

$$P(r)dr = r^2|R_{nl}(r)|^2 dr$$

This accounts for the $r^2$ factor from the volume element in spherical coordinates.

## Key Features

- **Exponential decay**: All wave functions decay as $e^{-Zr/na_0}$ at large $r$
- **Power law at origin**: $R \sim r^l$ as $r \to 0$
- **Nodes**: Number of radial nodes = $n - l - 1$
- **Normalization**: $\int_0^\infty r^2|R_{nl}|^2 dr = 1$

Related: [[Radial Nodes and Quantum Numbers]], [[Normalization of Radial Wave Functions]], [[Bohr Radius]], [[Spherical Harmonics Definition]]
