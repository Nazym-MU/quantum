## Problem
For large |y|, solve the asymptotic differential equation:
$$\frac{d^2\psi}{dy^2} \approx y^2\psi$$
Try exponential solutions of the form:
$$\psi(y) = e^{f(y)}$$
$$\frac{d\psi}{dy} = f'(y)e^{f(y)}$$
$$\frac{d^2\psi}{dy^2} = [f''(y) + (f'(y))^2]e^{f(y)}$$
Substituting into the differential equation:
$$[f''(y) + (f'(y))^2]e^{f(y)} = y^2 e^{f(y)}$$
$$f''(y) + (f'(y))^2 = y^2$$
## Large y Approximation
For large y, assume (f'(y))² dominates f''(y):
$$(f'(y))^2 \approx y^2$$
$$f'(y) \approx \pm y$$

Integrating:
$$f(y) \approx \pm \frac{y^2}{2}$$

Therefore:
$$\psi(y) \sim e^{\pm y^2/2}$$
## Physical Solution
Only ψ ∼ e^(-y²/2) is normalizable (∫|ψ|² dy must be finite).
The e^(+y²/2) solution grows exponentially and cannot represent a physical bound state.

## Related
- Used in: [[Ground State Wave Function Derivation]]
- Related to: [[Gaussian Wave Packet]]