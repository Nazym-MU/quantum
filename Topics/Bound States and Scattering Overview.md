Bound states occur when particles are confined to finite regions with E < V(∞). Energy is quantized due to boundary conditions.
## Core Concepts
- [[Bound States]] - localized, normalizable, discrete energies
- [[Unbound States]] - extended, continuous energies
- [[Boundary Conditions for Wave Functions]] - continuity requirements
- [[Energy Quantization from Boundary Conditions]] - why discrete energies
## Wave Function Behavior
**In classically allowed region (E > V):**
$$\frac{d^2\psi}{dx^2} = -k^2\psi \quad \Rightarrow \quad \text{oscillatory}$$
where k = √(2m(E-V))/ℏ
**In classically forbidden region (E < V):**
$$\frac{d^2\psi}{dx^2} = q^2\psi \quad \Rightarrow \quad \text{exponential}$$
where q = √(2m(V-E))/ℏ
→ Derivation: [[Square Well Solution Forms]]
**Turning point:** E = V(x), inflection point in ψ(x)
## Infinite Square Well
**Potential:**
$$V(x) = \begin{cases} 0 & |x| < a/2 \\ \infty & |x| > a/2 \end{cases}$$
**Energy eigenvalues:**
$$E_n = \frac{n^2\pi^2\hbar^2}{2ma^2}, \quad n = 1,2,3,...$$
→ Derivation: [[Particle in a Box Solution]]
**Quantization condition:** kₙa = nπ
**Node structure:** n-1 nodes for state |n⟩
See: [[Infinite Square Well (Particle in a Box)]]
## Finite Square Well
**Potential:**
$$V(x) = \begin{cases} 0 & |x| < a/2 \\ V_0 & |x| > a/2 \end{cases}$$

**Solution form:**
- Inside: oscillatory ψ(x) = A sin(kx) + B cos(kx)
- Outside: exponential decay ψ(x) ∝ e^(-q|x|)
**Transcendental equations for bound states:**
- Even: k tan(ka/2) = q
- Odd: k cot(ka/2) = -q
→ Derivation: [[Finite Square Well Bound State Conditions]]
**Key feature:** Wave function penetrates into classically forbidden region
See: [[Finite Square Well]]
## Scattering and Tunneling
### Probability Current
**Definition:**
$$j(x,t) = \frac{\hbar}{2mi}\left(\psi^*\frac{\partial\psi}{\partial x} - \psi\frac{\partial\psi^*}{\partial x}\right)$$
→ Derivation: [[Probability Current Derivation]]
**Conservation:** R + T = 1
→ Derivation: [[Probability Conservation R+T=1]]
See: [[Probability Current]]

### Potential Step

**E > V₀:** Partial reflection and transmission
- [[Reflection Coefficient]]: R < 1
- [[Transmission Coefficient]]: T = 1 - R
→ Derivation: [[Step Potential Solution]]

**E < V₀:** Total reflection but wave penetration
- R = 1, T = 0
- Wave decays as e^(-qx)

See: [[Potential Step Scattering]]

### Potential Barrier

**E < V₀:** Quantum tunneling
- Nonzero transmission through classically forbidden region
- Transmission: T ∝ e^(-2qa) for thick barriers
→ Derivation: [[Barrier Tunneling Solution]]

**E = V₀:** Special case
$$T = \frac{1}{1 + (ka/2)^2}$$
→ Derivation: [[Transmission Coefficient for Equal Energy and Barrier Height]]

See: [[Potential Barrier Scattering]], [[Quantum Tunneling]]

### Non-Square Barriers

For realistic potentials, use [[Non-Square Barrier Approximation]] (WKB method)

## Wave Propagation

- [[Plane Wave Direction of Travel]] - e^(ikx) travels right, e^(-ikx) travels left
- [[Wave Packets]] - realistic localized particles
- [[Momentum Eigenstates]] - plane waves as p eigenstates

## Key Results

1. Boundary conditions force energy quantization in bound states
2. Ground state has nonzero energy (zero-point energy)
3. Number of nodes increases with energy
4. Smaller confinement → larger energy spacing
5. Probability current is conserved: R + T = 1
6. Quantum tunneling allows transmission through barriers when E < V₀