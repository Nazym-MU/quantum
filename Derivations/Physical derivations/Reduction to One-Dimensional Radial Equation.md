## Starting Equation
Radial equation for $R(r)$:
$$
\left[
-\frac{\hbar^{2}}{2\mu}\left(\frac{d^{2}}{dr^{2}} + \frac{2}{r}\frac{d}{dr}\right)
+ \frac{l(l+1)\hbar^{2}}{2\mu r^{2}}
+ V(r)
\right] R(r)
= E R(r)
$$

# Substitution
Define $u(r) = r R(r)$, so $R(r) = u(r)/r$.
## First Derivative
$$
\frac{dR}{dr}
= \frac{d}{dr}\left(\frac{u}{r}\right)
= \frac{1}{r}\frac{du}{dr} - \frac{u}{r^{2}}
$$
## Second Derivative
$$
\frac{d^{2}R}{dr^{2}}
= \frac{d}{dr}\left( \frac{1}{r}\frac{du}{dr} - \frac{u}{r^{2}} \right)
$$
Compute term by term:
$$
= \frac{1}{r}\frac{d^{2}u}{dr^{2}}
- \frac{1}{r^{2}}\frac{du}{dr}
- \frac{d}{dr}\left( \frac{u}{r^{2}} \right)
$$
$$
= \frac{1}{r}\frac{d^{2}u}{dr^{2}}
- \frac{1}{r^{2}}\frac{du}{dr}
- \left( -\frac{2u}{r^{3}} + \frac{1}{r^{2}}\frac{du}{dr} \right)
$$
$$
= \frac{1}{r}\frac{d^{2}u}{dr^{2}}
- \frac{2}{r^{2}}\frac{du}{dr}
+ \frac{2u}{r^{3}}
$$
## Combination
$$
\frac{d^{2}R}{dr^{2}} + \frac{2}{r}\frac{dR}{dr}
$$
$$
= \left(\frac{1}{r}\frac{d^{2}u}{dr^{2}}
- \frac{2}{r^{2}}\frac{du}{dr}
+ \frac{2u}{r^{3}}\right)
+ \frac{2}{r}\left( \frac{1}{r}\frac{du}{dr} - \frac{u}{r^{2}} \right)
$$

$$
= \frac{1}{r}\frac{d^{2}u}{dr^{2}}
- \frac{2}{r^{2}}\frac{du}{dr}
+ \frac{2u}{r^{3}}
+ \frac{2}{r^{2}}\frac{du}{dr}
- \frac{2u}{r^{3}}
$$

$$
= \frac{1}{r}\frac{d^{2}u}{dr^{2}}
$$
### Substituting Back
$$
-\frac{\hbar^{2}}{2\mu}
\left(
\frac{d^{2}R}{dr^{2}} + \frac{2}{r}\frac{dR}{dr}
\right)
=
-\frac{\hbar^{2}}{2\mu}\frac{1}{r}\frac{d^{2}u}{dr^{2}}
$$
Multiplying the entire radial equation by $r$:

$$
-\frac{\hbar^{2}}{2\mu}\frac{d^{2}u}{dr^{2}}
+ \left[
\frac{l(l+1)\hbar^{2}}{2\mu r^{2}} + V(r)
\right] u(r)
= E u(r)
$$
## Final Form

$$
\left[
-\frac{\hbar^{2}}{2\mu}\frac{d^{2}}{dr^{2}}
+ V_{\text{eff}}(r)
\right] u(r)
= E u(r)
$$
where
$$
V_{\text{eff}}(r)
= \frac{l(l+1)\hbar^{2}}{2\mu r^{2}} + V(r)
$$
This is exactly the 1D time-independent Schrödinger equation.
## Boundary Condition
Since $R(r)$ must be finite at $r = 0$ and $R(r) = u(r)/r$, we require:
$$
u(0) = 0
$$
This is the standard boundary condition for the 1D Schrödinger equation on a half-line.
Related: [[Radial Schrödinger Equation]], [[Effective Potential in Central Force Problem]]
