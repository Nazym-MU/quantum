Spherical harmonics $Y_{l,m}(\theta, \phi)$ are the angular eigenfunctions of $\hat{L}^2$ and $\hat{L}_z$:
$$\hat{L}^2 Y_{l,m}(\theta, \phi) = l(l+1)\hbar^2 Y_{l,m}(\theta, \phi)$$
$$\hat{L}_z Y_{l,m}(\theta, \phi) = m\hbar Y_{l,m}(\theta, \phi)$$
In bra-ket notation: $\langle \theta, \phi | l, m \rangle = Y_{l,m}(\theta, \phi)$
## Role in Wave Functions
Complete energy eigenfunction for central potential:
$$\langle r, \theta, \phi | E, l, m \rangle = R_{nl}(r) Y_{l,m}(\theta, \phi)$$
The wave function **factorizes** into:
- **Radial part**: $R_{nl}(r)$ (depends on principal quantum number $n$ and $l$)
- **Angular part**: $Y_{l,m}(\theta, \phi)$ (depends only on $l$ and $m$)
## Quantum Numbers
- **$l$**: orbital angular momentum quantum number ($l = 0, 1, 2, 3, \ldots$)
- **$m$**: magnetic quantum number ($m = -l, -l+1, \ldots, l-1, l$)
For each $l$, there are $2l+1$ possible $m$ values.
## Notation
Spectroscopic notation for $l$ values:
- $l = 0$: s orbital (spherical)
- $l = 1$: p orbital (dumbbell)
- $l = 2$: d orbital
- $l = 3$: f orbital
## Properties
1. **Orthonormality**: $\int Y_{l',m'}^* Y_{l,m} d\Omega = \delta_{l,l'}\delta_{m,m'}$
2. **Completeness**: $\sum_{l,m} Y_{l,m}^*(\theta', \phi') Y_{l,m}(\theta, \phi) = \delta(\phi - \phi')\delta(\cos\theta - \cos\theta')$
3. **Parity**: $Y_{l,m}(\pi - \theta, \phi + \pi) = (-1)^l Y_{l,m}(\theta, \phi)$

Related: [[Explicit Spherical Harmonic Functions]], [[Normalization of Spherical Harmonics]], [[Probability Interpretation of Spherical Harmonics]]
