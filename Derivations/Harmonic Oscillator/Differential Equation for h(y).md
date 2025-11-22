## Starting Point
From [[TISE in Dimensionless Variables]], we have:
$$\frac{d^2\psi}{dy^2} = (y^2 - \varepsilon)\psi$$

Factor out exponential of the form e^(-y²/2) by writing:
$$\psi(y) = h(y)e^{-y^2/2}$$

## Why This Form?

The asymptotic solution (|y| → ∞) is ψ ~ e^(-y²/2). We're building this behavior into our ansatz from the start.

## Computing Derivatives

First derivative:
$$\frac{d\psi}{dy} = \frac{dh}{dy}e^{-y^2/2} + h\frac{d}{dy}(e^{-y^2/2})$$
$$= \frac{dh}{dy}e^{-y^2/2} - yhe^{-y^2/2}$$
$$= \left(\frac{dh}{dy} - yh\right)e^{-y^2/2}$$

Second derivative (using product rule on first derivative):
$$\frac{d^2\psi}{dy^2} = \frac{d}{dy}\left[\left(\frac{dh}{dy} - yh\right)e^{-y^2/2}\right]$$

$$= \left(\frac{d^2h}{dy^2} - \frac{dh}{dy} - yh'\right)e^{-y^2/2} + \left(\frac{dh}{dy} - yh\right)(-y)e^{-y^2/2}$$

$$= \left(\frac{d^2h}{dy^2} - \frac{dh}{dy} - \frac{dh}{dy} + y^2h\right)e^{-y^2/2}$$

$$= \left(\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + y^2h\right)e^{-y^2/2}$$

## Substituting into Schrödinger Equation

Original equation:
$$\frac{d^2\psi}{dy^2} = (y^2 - \varepsilon)\psi$$

Substitute ψ = he^(-y²/2) and its second derivative:
$$\left(\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + y^2h\right)e^{-y^2/2} = (y^2 - \varepsilon)he^{-y^2/2}$$

Divide by e^(-y²/2):
$$\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + y^2h = y^2h - \varepsilon h$$

Cancel y²h terms:
$$\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} = -\varepsilon h$$

## Final Result

$$\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + (\varepsilon - 1)h = 0$$

This is Eq. 7.103. The exponential factor has been "peeled off" leaving a simpler equation for h(y).

## Key Insight

By factoring out the problematic asymptotic behavior, the equation for h(y) is ready for power series solution. We expect h(y) to be a polynomial (doesn't blow up).

## Related
- Previous: [[Asymptotic Solution for Harmonic Oscillator]]
- Next: [[Power Series Recursion Relation for Hermite Polynomials]]
- Used in: [[Week 11.2 - Position Space Solution and Parity]]