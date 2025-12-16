**Principal quantum number**: $n = 1, 2, 3, \ldots$
**Orbital quantum number**: $l = 0, 1, 2, \ldots, n-1$
**Radial quantum number**: $n_r = n - l - 1 = 0, 1, 2, \ldots$
## Radial Nodes
The polynomial part of $u(r)$ is of degree $n_r$, which means it has **$n_r$ zeros** (roots).
These zeros are **radial nodes** - points where the radial wave function crosses zero.
**Number of radial nodes** = $n_r = n - l - 1$
## Examples
**Ground state** ($n=1, l=0$): $n_r = 0$ → no radial nodes
**First excited states** ($n=2$):
- $l=0$: $n_r = 1$ → one radial node
- $l=1$: $n_r = 0$ → no radial nodes
**Second excited states** ($n=3$):
- $l=0$: $n_r = 2$ → two radial nodes
- $l=1$: $n_r = 1$ → one radial node
- $l=2$: $n_r = 0$ → no radial nodes
## Physical Picture
**Maximum l states** ($l = n-1$): $n_r = 0$ → no nodes, single "bump" in probability
The radial probability density $r^2|R_{nl}(r)|^2$ has $n - l$ bumps:
- States with higher $n$ have more structure
- States with higher $l$ (for fixed $n$) have fewer nodes, one main bump farther out
## Radial Probability Distribution

For maximum $l$ states ($l = n-1$):

$$R_{n,n-1} \propto r^{n-1}e^{-Zr/na_0}$$

Probability density peaks at:
$$r_{\text{max}} = \frac{n^2 a_0}{Z}$$

This is exactly the Bohr radius for that shell!

## Connection to Classical Picture
Higher $n$ → larger average radius (outer shells)

Higher $l$ (for fixed $n$) → probability concentrated in one region farther from origin

Lower $l$ (for fixed $n$) → multiple bumps, some probability closer to nucleus (penetrating orbitals)

Related: [[Hydrogen Wave Functions]], [[Radial Wave Function Near Origin]], [[Degeneracy in Hydrogen Atom]]
