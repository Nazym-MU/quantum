Behavior of radial wave functions as $r \to 0$ and the boundary condition $u(0) = 0$.
## Setup
For central potential $V(r)$, the radial equation for $u(r) = rR(r)$ is:
$$\left[-\frac{\hbar^2}{2\mu}\frac{d^2}{dr^2} + \frac{l(l+1)\hbar^2}{2\mu r^2} + V(r)\right]u(r) = Eu(r)$$
## Power Series Analysis Near Origin
Assume $u(r) \sim r^s$ for small $r$. Substituting into the radial equation (keeping only most singular terms):
$$-\frac{\hbar^2}{2\mu}s(s-1)r^{s-2} + \frac{l(l+1)\hbar^2}{2\mu r^2}r^s = 0$$
$$s(s-1) = l(l+1)$$
**Solutions**: $s = l+1$ or $s = -l$
## Why s = -l is Forbidden
**For $l \geq 1$**: $u \sim r^{-l}$ means $R = u/r \sim r^{-l-1}$
Normalization integral:
$$\int_0^\infty r^2|R|^2 dr = \int_0^\infty r^{-2l} dr$$
This diverges at $r = 0$ for $l \geq 1$ → cannot be normalized → forbidden.
**For $l = 0$**: $u \sim$ constant means $R \sim 1/r$
From electrostatics: $\nabla^2(1/r) = -4\pi\delta^3(\mathbf{r})$
This creates a delta function at origin, which violates Schrödinger equation for smooth potentials like Coulomb → forbidden.
## Boundary Condition
Only allowed solution: $s = l+1$
$$u(r) \sim r^{l+1} \text{ as } r \to 0$$
Therefore: **$u(0) = 0$** for all $l \geq 0$
This is the boundary condition at the origin for the radial wave function.
## Physical Consequence
Since $R(r) = u(r)/r$:
$$R(r) \sim r^l \text{ as } r \to 0$$
- **$l = 0$**: $R$ is finite at origin (s orbitals can reach nucleus)
- **$l \geq 1$**: $R \to 0$ at origin (p, d, f orbitals vanish at nucleus)
This explains why positronium (electron-positron bound state) can only annihilate in $l=0$ states - the particles must overlap spatially.

Related: [[Centrifugal Barrier]], [[Boundary Condition u(0) = 0 Derivation]], [[Normalization of Radial Wave Functions]]
