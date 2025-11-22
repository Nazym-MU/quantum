# Probability Current Derivation

## Goal
Derive the probability current j_x and show it satisfies a local conservation law.

## Starting Point
Time-dependent [[Schrödinger Equation (Time-Dependent)]]:
$$i\hbar\frac{\partial\psi}{\partial t} = -\frac{\hbar^2}{2m}\frac{\partial^2\psi}{\partial x^2} + V(x)\psi$$

## Step 1: Time Derivative of Probability Density

Consider ∂(ψ*ψ)/∂t. Using product rule:
$$\frac{\partial(\psi^*\psi)}{\partial t} = \psi^*\frac{\partial\psi}{\partial t} + \psi\frac{\partial\psi^*}{\partial t}$$

## Step 2: Express Time Derivatives

From Schrödinger equation:
$$\frac{\partial\psi}{\partial t} = \frac{1}{i\hbar}\left[-\frac{\hbar^2}{2m}\frac{\partial^2\psi}{\partial x^2} + V(x)\psi\right]$$

Taking complex conjugate:
$$\frac{\partial\psi^*}{\partial t} = \frac{-1}{i\hbar}\left[-\frac{\hbar^2}{2m}\frac{\partial^2\psi^*}{\partial x^2} + V(x)\psi^*\right]$$

(V is real, so V* = V)

## Step 3: Substitute and Simplify

$$\frac{\partial(\psi^*\psi)}{\partial t} = \frac{1}{i\hbar}\left[\psi^*\left(-\frac{\hbar^2}{2m}\frac{\partial^2\psi}{\partial x^2} + V\psi\right) - \psi\left(-\frac{\hbar^2}{2m}\frac{\partial^2\psi^*}{\partial x^2} + V\psi^*\right)\right]$$

The V terms cancel: Vψ*ψ - Vψψ* = 0

$$\frac{\partial(\psi^*\psi)}{\partial t} = \frac{1}{i\hbar}\left[-\frac{\hbar^2}{2m}\left(\psi^*\frac{\partial^2\psi}{\partial x^2} - \psi\frac{\partial^2\psi^*}{\partial x^2}\right)\right]$$

$$= -\frac{\hbar}{2mi}\left(\psi^*\frac{\partial^2\psi}{\partial x^2} - \psi\frac{\partial^2\psi^*}{\partial x^2}\right)$$

## Step 4: Recognize as Divergence

The right side can be written as:
$$-\frac{\partial}{\partial x}\left[\frac{\hbar}{2mi}\left(\psi^*\frac{\partial\psi}{\partial x} - \psi\frac{\partial\psi^*}{\partial x}\right)\right]$$

To verify, differentiate the expression in brackets:
$$\frac{\partial}{\partial x}\left[\psi^*\frac{\partial\psi}{\partial x} - \psi\frac{\partial\psi^*}{\partial x}\right] = \frac{\partial\psi^*}{\partial x}\frac{\partial\psi}{\partial x} + \psi^*\frac{\partial^2\psi}{\partial x^2} - \frac{\partial\psi}{\partial x}\frac{\partial\psi^*}{\partial x} - \psi\frac{\partial^2\psi^*}{\partial x^2}$$

The cross terms cancel, leaving:
$$= \psi^*\frac{\partial^2\psi}{\partial x^2} - \psi\frac{\partial^2\psi^*}{\partial x^2}$$

## Step 5: Define Probability Current

Define:
$$j_x = \frac{\hbar}{2mi}\left(\psi^*\frac{\partial\psi}{\partial x} - \psi\frac{\partial\psi^*}{\partial x}\right)$$

Then we have the **continuity equation**:
$$\frac{\partial(\psi^*\psi)}{\partial t} + \frac{\partial j_x}{\partial x} = 0$$

## Step 6: Integral Form

Integrate over region [a, b]:
$$\frac{d}{dt}\int_a^b |\psi|^2 dx = \int_a^b \frac{\partial(\psi^*\psi)}{\partial t} dx = -\int_a^b \frac{\partial j_x}{\partial x} dx$$

By fundamental theorem of calculus:
$$\frac{d}{dt}\int_a^b |\psi|^2 dx = -[j_x(b,t) - j_x(a,t)] = j_x(a,t) - j_x(b,t)$$

**Interpretation:** Probability in [a,b] increases due to net inward current flow.

## For Plane Waves

If ψ = Ae^(ikx) + Be^(-ikx), then:
- ∂ψ/∂x = ikAe^(ikx) - ikBe^(-ikx)
- ψ* = A*e^(-ikx) + B*e^(ikx)
- ∂ψ*/∂x = -ikA*e^(-ikx) + ikB*e^(ikx)

Computing ψ*∂ψ/∂x (4 terms):
$$\psi^*\frac{\partial\psi}{\partial x} = ik|A|^2 + ik(AB^*e^{2ikx} - A^*Be^{-2ikx}) - ik|B|^2$$

Computing ψ∂ψ*/∂x (4 terms):
$$\psi\frac{\partial\psi^*}{\partial x} = -ik|A|^2 - ik(AB^*e^{2ikx} - A^*Be^{-2ikx}) + ik|B|^2$$

Subtracting:
$$\psi^*\frac{\partial\psi}{\partial x} - \psi\frac{\partial\psi^*}{\partial x} = 2ik(|A|^2 - |B|^2)$$

Therefore:
$$j_x = \frac{\hbar}{2mi} \cdot 2ik(|A|^2 - |B|^2) = \frac{\hbar k}{m}(|A|^2 - |B|^2)$$

## Physical Meaning
- j_x > 0: net probability flow to the right
- j_x < 0: net probability flow to the left
- j_x = 0: no net flow (stationary or standing wave)

## Related
- [[Probability Current]]
- [[Reflection Coefficient]]
- [[Transmission Coefficient]]