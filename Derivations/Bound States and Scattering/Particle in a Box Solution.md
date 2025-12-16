**Problem:** Solve TISE for infinite square well V(x) = 0 for |x| < a/2, V(x) = ∞ for |x| > a/2.
**Step 1: Inside the well (|x| < a/2)**
Schrödinger equation:
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} = E\psi$$
$$\frac{d^2\psi}{dx^2} = -k^2\psi, \quad k = \sqrt{2mE/\hbar^2}$$
**Step 2: General solution**
$$\psi(x) = A\sin(kx) + B\cos(kx)$$
**Step 3: Apply boundary conditions**
At x = -a/2: ψ(-a/2) = 0
$$A\sin(-ka/2) + B\cos(-ka/2) = 0$$
$$-A\sin(ka/2) + B\cos(ka/2) = 0 \quad \text{...(1)}$$

At x = a/2: ψ(a/2) = 0
$$A\sin(ka/2) + B\cos(ka/2) = 0 \quad \text{...(2)}$$

**Step 4: Matrix form**
$$\begin{pmatrix} \sin(ka/2) & \cos(ka/2) \\ -\sin(ka/2) & \cos(ka/2) \end{pmatrix} \begin{pmatrix} A \\ B \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$$
**Step 5: Nontrivial solutions**

For nonzero A, B, determinant must vanish:
$$\sin(ka/2)\cos(ka/2) - (-\sin(ka/2)\cos(ka/2)) = 0$$
$$2\sin(ka/2)\cos(ka/2) = 0$$
$$\sin(ka) = 0$$

Therefore:
$$ka = n\pi, \quad n = 1,2,3,...$$

**Step 6: Two solution types**

**For n = 1,3,5,... (odd):** ka/2 = π/2, 3π/2, ...
- cos(ka/2) = 0
- From equation (1): A = 0
- Solution: ψₙ(x) = Bₙ cos(nπx/a)

**For n = 2,4,6,... (even):** ka/2 = π, 2π, ...
- sin(ka/2) = 0  
- From equation (1): B = 0
- Solution: ψₙ(x) = Aₙ sin(nπx/a)

**Step 7: Normalization**

$$\int_{-a/2}^{a/2} |\psi_n(x)|^2 dx = 1$$

For both sin and cos:
$$|A_n|^2 \int_{-a/2}^{a/2} \sin^2(n\pi x/a) dx = |A_n|^2 \cdot \frac{a}{2} = 1$$

Therefore: Aₙ = Bₙ = √(2/a)

**Step 8: Energy eigenvalues**

From kₙ = nπ/a:
$$k_n^2 = \frac{n^2\pi^2}{a^2} = \frac{2mE_n}{\hbar^2}$$

$$E_n = \frac{n^2\pi^2\hbar^2}{2ma^2}$$

**Final Result:**

**Energy eigenfunctions:**
$$\psi_n(x) = \begin{cases} \sqrt{2/a}\cos(n\pi x/a) & n \text{ odd} \\ \sqrt{2/a}\sin(n\pi x/a) & n \text{ even} \end{cases}$$

**Energy eigenvalues:**
$$E_n = \frac{n^2\pi^2\hbar^2}{2ma^2}, \quad n = 1,2,3,...$$

**Related:** [[Infinite Square Well (Particle in a Box)]]