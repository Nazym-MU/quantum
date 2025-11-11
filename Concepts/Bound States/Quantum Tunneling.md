**Definition:** Quantum penetration of a particle into or through a classically forbidden region where E < V(x).

**Physical Mechanism:**
Classically: particle with E < V cannot enter region (would require negative kinetic energy).

Quantum mechanically: wave function doesn't vanish abruptly but decays exponentially.

**Mathematical Form:**
In region where E < V(x):
$$\frac{d^2\psi}{dx^2} = q^2\psi, \quad q = \sqrt{2m[V(x)-E]/\hbar^2}$$

Solution: ψ(x) ∝ e^(-qx) (exponential decay)

**Penetration Depth:**
Characteristic length scale: δ ~ 1/q ~ ℏ/√(2m(V-E))

Higher barrier or larger energy difference → faster decay.

**Tunneling Through Barriers:**
For finite-width barrier (width a), nonzero transmission occurs:
$$T \approx e^{-2qa} \quad \text{for } qa \gg 1$$

See [[Potential Barrier Scattering]] for complete analysis.

**Physical Consequences:**
- Enables barrier penetration and quantum tunneling
- [[Bound States]] have wave function "tails" outside potential well
- Finite probability to find particle in classically forbidden region

**Examples:**
- [[Finite Square Well]]: exponential tails outside well
- [[Potential Barrier Scattering]]: transmission for E < V₀
- Alpha decay from atomic nuclei
- Scanning tunneling microscope
- Field emission from metals

**Contrast with Classical:**
Classical particle reflects at turning point where E = V(x). Quantum particle has nonzero amplitude beyond this point.