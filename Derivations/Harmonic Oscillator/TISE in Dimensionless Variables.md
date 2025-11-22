## Starting Point
Position-space time-independent Schrödinger equation:
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + \frac{1}{2}m\omega^2x^2\psi(x) = E\psi(x)$$
## Dimensionless Position
Define:
$$y = \sqrt{\frac{m\omega}{\hbar}} x$$
## Change of Variables
Since y = √(mω/ℏ) x, we have x = √(ℏ/mω) y, so:
$$\frac{d}{dx} = \frac{dy}{dx}\frac{d}{dy} = \sqrt{\frac{m\omega}{\hbar}}\frac{d}{dy}$$
$$\frac{d^2}{dx^2} = \frac{m\omega}{\hbar}\frac{d^2}{dy^2}$$
## Substituting into Schrödinger Equation
$$-\frac{\hbar^2}{2m}\frac{m\omega}{\hbar}\frac{d^2\psi}{dy^2} + \frac{1}{2}m\omega^2\frac{\hbar}{m\omega}y^2\psi = E\psi$$
Simplify:
$$-\frac{\hbar\omega}{2}\frac{d^2\psi}{dy^2} + \frac{1}{2}\hbar\omega y^2\psi = E\psi$$
Divide by ℏω/2:
$$-\frac{d^2\psi}{dy^2} + y^2\psi = \frac{2E}{\hbar\omega}\psi$$
## Dimensionless Energy
Define:
$$\varepsilon = \frac{2E}{\hbar\omega}$$

## Final Form

$$\frac{d^2\psi}{dy^2} = (y^2 - \varepsilon)\psi$$
## Related
- Used in: [[Week 11.2 - Position Space Solution and Parity]]
- Next step: [[Asymptotic Solution for Harmonic Oscillator]]