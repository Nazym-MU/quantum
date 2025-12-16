Complete derivation of why radial wave function must satisfy $u(0) = 0$.
## Starting Point
Radial equation for $u(r) = rR(r)$:
$$-\frac{\hbar^2}{2\mu}\frac{d^2u}{dr^2} + \left[\frac{l(l+1)\hbar^2}{2\mu r^2} + V(r)\right]u = Eu$$
## Assumption for Small r
Near origin, assume potential $V(r)$ is not more singular than $1/r^2$.
For Coulomb: $V(r) = -Ze^2/r$ satisfies this.
Try solution: $u(r) \sim r^s$
## Derivatives
$$\frac{du}{dr} = sr^{s-1}$$
$$\frac{d^2u}{dr^2} = s(s-1)r^{s-2}$$
## Substitution into Equation
Near origin, dominant terms:
$$-\frac{\hbar^2}{2\mu}s(s-1)r^{s-2} + \frac{l(l+1)\hbar^2}{2\mu r^2}r^s = 0$$
$$-s(s-1)r^{s-2} + l(l+1)r^{s-2} = 0$$
## Indicial Equation
$$s(s-1) = l(l+1)$$
$$s^2 - s - l^2 - l = 0$$
$$s^2 - s - l(l+1) = 0$$

Factoring:
$$(s - l - 1)(s + l) = 0$$

**Solutions**: $s = l+1$ or $s = -l$

## Testing s = -l

**Case 1: $l \geq 1$**

$u \sim r^{-l}$ implies $R = u/r \sim r^{-l-1}$

Normalization integral:
$$\int_0^\infty r^2|R|^2 dr = \int_0^\infty r^{2-2l-2} dr = \int_0^\infty r^{-2l} dr$$

For $l \geq 1$: exponent $-2l \leq -2$

Lower limit: $\lim_{r\to 0} r^{-2l+1} = \lim_{r\to 0} r^{\text{negative}} = \infty$

**Integral diverges → cannot normalize → FORBIDDEN**

**Case 2: $l = 0$**

$u \sim r^0 =$ constant, so $R \sim 1/r$

From electrostatics (Poisson equation):
$$\nabla^2\left(\frac{1}{r}\right) = -4\pi\delta^3(\mathbf{r})$$

Full 3D Schrödinger equation:
$$-\frac{\hbar^2}{2\mu}\nabla^2 R + V(r)R = ER$$

If $R \sim 1/r$, then $\nabla^2 R$ has **delta function at origin**.

For smooth $V(r)$ (like Coulomb), this is inconsistent.

**FORBIDDEN for physical potentials**

## Conclusion

Only allowed: $s = l + 1$

$$u(r) \sim r^{l+1} \text{ as } r \to 0$$

Therefore:
$$\boxed{u(0) = 0}$$

This is the **boundary condition at origin** for all bound state solutions.

## Physical Consequence

$$R(r) = \frac{u(r)}{r} \sim r^l \text{ as } r \to 0$$

- $l = 0$: $R(0)$ finite (s orbitals reach nucleus)
- $l > 0$: $R(0) = 0$ (centrifugal barrier keeps particle away)

Related: [[Radial Wave Function Near Origin]], [[Centrifugal Barrier]], [[Normalization of Radial Wave Functions]]
