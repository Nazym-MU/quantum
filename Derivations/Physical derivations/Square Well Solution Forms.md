**Goal:** Show why we get oscillatory solutions inside well and exponential solutions outside.

**Inside Well (E > V):**

TISE: $-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V\psi = E\psi$

Rearrange: $\frac{d^2\psi}{dx^2} = -\frac{2m(E-V)}{\hbar^2}\psi = -k^2\psi$

where $k^2 = \frac{2m(E-V)}{\hbar^2} > 0$ (positive since E > V)

**Solving d²ψ/dx² = -k²ψ:**

Try ψ = e^(rx):
$$r^2 e^{rx} = -k^2 e^{rx}$$
$$r^2 = -k^2$$
$$r = \pm ik$$

General solution:
$$\psi(x) = C_1 e^{ikx} + C_2 e^{-ikx}$$

Using Euler's formula e^(iθ) = cos θ + i sin θ:
$$\psi(x) = A\sin(kx) + B\cos(kx)$$

**Result:** Oscillatory with wavelength λ = 2π/k

---

**Outside Well (E < V):**

Rearrange: $\frac{d^2\psi}{dx^2} = +\frac{2m(V-E)}{\hbar^2}\psi = +q^2\psi$

where $q^2 = \frac{2m(V-E)}{\hbar^2} > 0$ (positive since V > E)

**Solving d²ψ/dx² = +q²ψ:**

Try ψ = e^(rx):
$$r^2 e^{rx} = q^2 e^{rx}$$
$$r^2 = q^2$$
$$r = \pm q$$

General solution:
$$\psi(x) = C e^{qx} + D e^{-qx}$$

**Normalizability constraint:**

For x → +∞: must discard e^(qx) (grows without bound)
$$\psi(x) = D e^{-qx}, \quad x > a/2$$

For x → -∞: must discard e^(-qx) (grows without bound)  
$$\psi(x) = C e^{qx}, \quad x < -a/2$$

**Result:** Exponential decay with penetration depth δ ~ 1/q

---

**Summary:**

| Region | Condition | d²ψ/dx² | Solution Type |
|--------|-----------|---------|---------------|
| E > V  | k² > 0    | -k²ψ    | Oscillatory   |
| E < V  | q² > 0    | +q²ψ    | Exponential   |

**Physical Interpretation:**
- E > V: Positive kinetic energy → wavelike propagation
- E < V: Classically forbidden → quantum tunneling with exponential decay

**Related:** [[Finite Square Well]], [[Quantum Tunneling]]