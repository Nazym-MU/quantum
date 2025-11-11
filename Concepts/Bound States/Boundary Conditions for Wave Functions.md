**General Requirements:**

**1. Continuity of ψ(x):**
Wave function must be continuous everywhere (unless V is infinite).

**2. Continuity of dψ/dx:**
First derivative must be continuous at boundaries where V is finite.

**Derivation from Schrödinger Equation:**
Integrate TISE across small interval [x-ε, x+ε]:
$$\int_{x-\varepsilon}^{x+\varepsilon} \frac{d^2\psi}{dx^2} dx = \frac{2m}{\hbar^2}\int_{x-\varepsilon}^{x+\varepsilon}[V(x)-E]\psi(x) dx$$

Left side: dψ/dx|_(x+ε) - dψ/dx|_(x-ε)

Right side → 0 as ε → 0 for finite V.

Therefore: dψ/dx is continuous at finite potential steps.

**Special Cases:**

**Infinite Potential Wall:**
- ψ = 0 at wall
- dψ/dx can be discontinuous
- Example: [[Infinite Square Well (Particle in a Box)]]

**Finite Potential Step:**
- Both ψ and dψ/dx continuous
- Example: [[Finite Square Well]]

**Physical Interpretation:**
Continuity ensures probability current is conserved and wave function represents a physically realizable state.

**Related:**
- [[Energy Quantization from Boundary Conditions]]
- [[Bound States]]