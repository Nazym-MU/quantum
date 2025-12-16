The effective repulsive potential arising from orbital angular momentum.
In the radial equation, the centrifugal term appears as:
$$V_{\text{centrifugal}}(r) = \frac{l(l+1)\hbar^2}{2\mu r^2}$$
This combines with the actual potential $V(r)$ to give the **effective potential**:
$$V_{\text{eff}}(r) = \frac{l(l+1)\hbar^2}{2\mu r^2} + V(r)$$
## Physical Origin
Classically, a particle with angular momentum $L$ rotating at distance $r$ has rotational kinetic energy:

$$T_{\text{rot}} = \frac{L^2}{2I} = \frac{L^2}{2\mu r^2}$$
where $I = \mu r^2$ is the moment of inertia.
In quantum mechanics: $L^2 = l(l+1)\hbar^2$, giving the centrifugal term.
## Effect on Wave Function
The centrifugal barrier acts as a **repulsive force** pushing the particle away from the origin.
**Higher $l$**: Stronger barrier → particle less likely near origin
This forces the wave function to vanish more rapidly at origin:
$$u(r) \sim r^{l+1} \text{ as } r \to 0$$
## Comparison for Different l
For Coulomb potential $V(r) = -Ze^2/r$:
$$V_{\text{eff}} = \frac{l(l+1)\hbar^2}{2\mu r^2} - \frac{Ze^2}{r}$$
- **$l = 0$**: No barrier, just Coulomb attraction
- **$l = 1$**: Small barrier, creates "bump" near origin
- **$l = 2, 3, ...$**: Progressively stronger barriers
At small $r$, the $1/r^2$ term dominates over the $1/r$ term, creating effective repulsion.
## Physical Applications
**Positronium annihilation**: Electron and positron can only annihilate in $l=0$ states because they must overlap spatially. For $l > 0$, the centrifugal barrier keeps them apart.
**Chemical bonding**: s orbitals ($l=0$) penetrate closer to nucleus than p or d orbitals, affecting screening in multi-electron atoms.
**Nuclear physics**: Important for understanding nuclear reactions and bound states.

Related: [[Effective Potential in Central Force Problem]], [[Radial Wave Function Near Origin]], [[Radial Schrödinger Equation]]
