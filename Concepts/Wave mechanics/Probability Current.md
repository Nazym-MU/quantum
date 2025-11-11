# Probability Current

## Physical Meaning
The flow of probability per unit time through a point in space. Ensures local conservation: probability cannot teleport from one location to another but must flow continuously through intermediate points.

## Mathematical Definition
$$j_x = \frac{\hbar}{2mi}\left(\psi^* \frac{\partial \psi}{\partial x} - \psi \frac{\partial \psi^*}{\partial x}\right)$$

## Conservation Law
$$\frac{\partial}{\partial t}(\psi^*\psi) + \frac{\partial j_x}{\partial x} = 0$$

This is the continuity equation for probability. Integrating over region [a, b]:
$$\frac{d}{dt}\int_a^b |\psi|^2 dx = j_x(a,t) - j_x(b,t)$$

Probability in a region changes only due to net flow through boundaries.

## For Plane Waves
For ψ = Ae^(ikx) + Be^(-ikx):
$$j_x = \frac{\hbar k}{m}(|A|^2 - |B|^2)$$

- |A|² term: rightward current
- |B|² term: leftward current
- Net current: difference

## For Exponential Decay
For real exponential ψ = Ce^(-qx), the current vanishes:
$$j_x = 0$$
No probability flow even though ψ ≠ 0.

## Applications
- Defining [[Reflection Coefficient]]: R = |j_ref|/j_inc
- Defining [[Transmission Coefficient]]: T = j_trans/j_inc  
- Analyzing [[Potential Step Scattering]] and [[Potential Barrier Scattering]]

## Derivation
See [[Probability Current Derivation]] for step-by-step calculation from [[Schrödinger Equation (Time-Dependent)]].