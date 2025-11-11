**Definition:** Potential energy:
$$V(x) = \begin{cases} 0 & |x| < a/2 \\ V_0 & |x| > a/2 \end{cases}$$

For [[Bound States]], consider 0 < E < V₀.

**Three-Region Solution:**

**Inside well (|x| < a/2):** E > V, oscillatory behavior
$$\frac{d^2\psi}{dx^2} = -k^2\psi, \quad k = \sqrt{2mE/\hbar^2}$$
$$\psi(x) = A\sin(kx) + B\cos(kx)$$

**Outside well (|x| > a/2):** E < V, exponential decay
$$\frac{d^2\psi}{dx^2} = q^2\psi, \quad q = \sqrt{2m(V_0-E)/\hbar^2}$$
$$\psi(x) = \begin{cases} Ce^{qx} & x < -a/2 \\ De^{-qx} & x > a/2 \end{cases}$$

Discard growing exponentials (e^(-qx) for x < -a/2, e^(qx) for x > a/2) to ensure normalizability.

**Matching Conditions:**
At x = ±a/2, both ψ(x) and dψ/dx must be continuous. This constrains the allowed energies to discrete values.

**Key Features:**
- Only certain E values allow smooth matching → energy quantization
- Lower energy → fewer nodes in ψ(x)
- Wave function penetrates into classically forbidden region

**Related:**
- [[Quantum Tunneling]]
- [[Infinite Square Well (Particle in a Box)]]
- [[Boundary Conditions for Wave Functions]]