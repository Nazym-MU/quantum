## Position-Space Wave Function
$$\psi(x) = \frac{1}{(\pi a^2)^{1/4}}e^{-x^2/(2a^2)}$$
where a is the width parameter.
## Momentum-Space Wave Function
$$\tilde{\psi}(p) = \frac{a^{1/2}}{(\pi\hbar^2)^{1/4}}e^{-p^2a^2/(2\hbar^2)}$$
Both are Gaussians (unique to Gaussian wave packets).
## Probability Densities
**Position:**
$$|\psi(x)|^2 = \frac{1}{\sqrt{\pi a^2}}e^{-x^2/a^2}$$
**Momentum:**
$$|\tilde{\psi}(p)|^2 = \frac{a}{\sqrt{\pi\hbar^2}}e^{-p^2a^2/\hbar^2}$$
## Computing Uncertainties
**Position uncertainty:**
- ⟨x⟩ = 0 (by symmetry, integrand is odd)
- ⟨x²⟩ = a²/2 (use Gaussian integral)
- Δx = √(⟨x²⟩ - ⟨x⟩²) = a/√2
**Momentum uncertainty:**
- ⟨pₓ⟩ = 0 (by symmetry)
- ⟨p²ₓ⟩ = ℏ²/(2a²)
- Δpₓ = ℏ/(√2 a)
## Minimum Uncertainty
$$\Delta x \cdot \Delta p_x = \frac{a}{\sqrt{2}} \cdot \frac{\hbar}{\sqrt{2}a} = \frac{\hbar}{2}$$
This saturates the Heisenberg uncertainty principle. Gaussians are minimum uncertainty states.
## Effect of Parameter a
**Larger a:**
- Broader in position space (larger Δx)
- Narrower in momentum space (smaller Δp)
- Product ΔxΔp = ℏ/2 remains constant
**Smaller a:**
- Narrower in position space (smaller Δx)
- Broader in momentum space (larger Δp)
- As a → 0: approaches δ(x) in position, constant in momentum
## Gaussian Integral Formulas
$$\int_{-\infty}^{\infty} e^{-x^2/a^2} dx = a\sqrt{\pi}$$
$$\int_{-\infty}^{\infty} x^2 e^{-x^2/a^2} dx = \frac{a^3\sqrt{\pi}}{2}$$