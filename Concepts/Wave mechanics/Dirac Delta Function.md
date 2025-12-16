## Definition
The Dirac delta function δ(x-x') is not a true function but a distribution with:
$$\delta(x-x') = \begin{cases} \infty & x = x' \\ 0 & x \neq x' \end{cases}$$

## Key Property: Sifting/Sampling
$$\int_{-\infty}^{\infty} f(x)\delta(x-x') dx = f(x')$$

The delta "picks out" the value of f at x = x'.
## Normalization
$$\int_{-\infty}^{\infty} \delta(x-x') dx = 1$$
## Physical Interpretation as Limit
Think of δ(x-x') as the limit of increasingly narrow, tall peaks:
- Gaussian: δ(x) = lim[ε→0] (1/√(πε))e^(-x²/ε)
- Rectangle: width ε, height 1/ε, as ε→0
- All have unit area
## Role in Position Eigenstates
$$\langle x|x'\rangle = \delta(x-x')$$

This ensures:
- Orthogonality: ⟨x|x'⟩ = 0 when x ≠ x'
- Proper resolution of identity: ∫dx |x⟩⟨x| = Î

## Other Representations
$$\delta(x-x') = \frac{1}{2\pi\hbar}\int_{-\infty}^{\infty} e^{ip(x-x')/\hbar} dp$$

This connects position and momentum basis states.