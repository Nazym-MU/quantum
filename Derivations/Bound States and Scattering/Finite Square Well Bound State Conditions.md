# Finite Square Well Bound State Conditions

## Problem
Derive the transcendental equations that determine bound state energies for the [[Finite Square Well]].

## Potential
$$V(x) = \begin{cases} 0 & |x| < a/2 \\ V_0 & |x| > a/2 \end{cases}$$

Consider bound states with 0 < E < V₀.

## Wave Functions

From [[Square Well Solution Forms]]:

**Inside (|x| < a/2):**
$$\psi_{in}(x) = A\sin(kx) + B\cos(kx)$$
where k = √(2mE)/ℏ

**Outside (|x| > a/2):**
$$\psi_{out}(x) = \begin{cases} Ce^{qx} & x < -a/2 \\ De^{-qx} & x > a/2 \end{cases}$$
where q = √(2m(V₀-E))/ℏ

## Use Symmetry

Potential is symmetric: V(-x) = V(x)

Therefore, eigenstates have definite [[Parity Operator|parity]]:
- **Even solutions:** ψ(-x) = ψ(x)
- **Odd solutions:** ψ(-x) = -ψ(x)

## Even Solutions (ψ(-x) = ψ(x))

**Form:**
$$\psi(x) = \begin{cases} Ae^{qx} & x < -a/2 \\ B\cos(kx) & |x| < a/2 \\ Ae^{-qx} & x > a/2 \end{cases}$$

(Symmetry forces: C = D = A, and sine term vanishes)

**Boundary conditions at x = a/2:**

Continuity of ψ:
$$B\cos(ka/2) = Ae^{-qa/2}$$

Continuity of dψ/dx:
$$-kB\sin(ka/2) = -qAe^{-qa/2}$$

Divide second by first:
$$k\tan(ka/2) = q$$

## Odd Solutions (ψ(-x) = -ψ(x))

**Form:**
$$\psi(x) = \begin{cases} -Ae^{qx} & x < -a/2 \\ B\sin(kx) & |x| < a/2 \\ Ae^{-qx} & x > a/2 \end{cases}$$

(Symmetry forces: D = -C = A, and cosine term vanishes)

**Boundary conditions at x = a/2:**

Continuity of ψ:
$$B\sin(ka/2) = Ae^{-qa/2}$$

Continuity of dψ/dx:
$$kB\cos(ka/2) = -qAe^{-qa/2}$$

Divide second by first:
$$-k\cot(ka/2) = q$$

or equivalently:
$$k\tan(ka/2) = -q$$

But tan is negative when cot is positive, so write as:
$$-k\cot(ka/2) = q$$

## Summary of Transcendental Equations

**Even states:**
$$k\tan\left(\frac{ka}{2}\right) = q$$

**Odd states:**
$$k\cot\left(\frac{ka}{2}\right) = -q$$

where:
$$k = \sqrt{\frac{2mE}{\hbar^2}}, \quad q = \sqrt{\frac{2m(V_0-E)}{\hbar^2}}$$

## Constraint Equation

Note that:
$$k^2 + q^2 = \frac{2mE}{\hbar^2} + \frac{2m(V_0-E)}{\hbar^2} = \frac{2mV_0}{\hbar^2} = \text{constant}$$

Define dimensionless parameters:
$$\xi = \frac{ka}{2}, \quad \eta = \frac{qa}{2}$$

Then:
$$\xi^2 + \eta^2 = \frac{mV_0 a^2}{2\hbar^2} \equiv z_0^2$$

The transcendental equations become:
- **Even:** ξ tan ξ = η
- **Odd:** ξ cot ξ = -η

subject to: ξ² + η² = z₀²

## Graphical Solution

These are typically solved graphically by plotting:
1. Circle: ξ² + η² = z₀² (constraint)
2. Even curve: η = ξ tan ξ
3. Odd curve: η = -ξ cot ξ

Intersections give bound state energies.

## Number of Bound States

The number of bound states depends on z₀ = (a/2)√(2mV₀)/ℏ:
- At least one bound state always exists (ground state, even)
- For n bound states: (n-1)π/2 < z₀ < nπ/2

**Deep well limit (V₀ → ∞):**
Approaches [[Infinite Square Well (Particle in a Box)]]

## Physical Insight

- Matching boundary conditions quantizes E
- Cannot solve analytically (transcendental equations)
- Graphical or numerical methods required
- Finite well has fewer bound states than infinite well
- Wave function penetrates into classically forbidden region

## Related
- [[Finite Square Well]]
- [[Boundary Conditions for Wave Functions]]
- [[Energy Quantization from Boundary Conditions]]
- [[Square Well Solution Forms]]