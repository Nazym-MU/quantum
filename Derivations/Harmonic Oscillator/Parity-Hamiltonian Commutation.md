## Condition for Commutation

Two operators commute when their order doesn't matter:
$$[\hat{\Pi}, \hat{H}] = \hat{\Pi}\hat{H} - \hat{H}\hat{\Pi} = 0$$

## Computing [Π̂, Ĥ] in Position Space

Apply both orderings to arbitrary state |ψ⟩ and project onto ⟨x|:

### First Ordering: Π̂Ĥ

$$\langle x|\hat{\Pi}\hat{H}|\psi\rangle = \langle -x|\hat{H}|\psi\rangle$$

Using position-space Hamiltonian:
$$= \left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2} + V(-x)\right]\psi(-x)$$

### Second Ordering: ĤΠ̂

$$\langle x|\hat{H}\hat{\Pi}|\psi\rangle = \hat{H}_x [\langle x|\hat{\Pi}|\psi\rangle]$$

where Ĥₓ acts on position x:
$$= \left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2} + V(x)\right]\psi(-x)$$

### Comparing

For these to be equal:
$$\left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2} + V(-x)\right]\psi(-x) = \left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2} + V(x)\right]\psi(-x)$$

Kinetic terms match. Potential terms match if:
$$V(-x) = V(x)$$

**This is Eq. 7.120 result**.

## Harmonic Oscillator

$$V(x) = \frac{1}{2}m\omega^2 x^2$$

Check:
$$V(-x) = \frac{1}{2}m\omega^2 (-x)^2 = \frac{1}{2}m\omega^2 x^2 = V(x)$$ ✓

**Therefore**: [Π̂, Ĥ] = 0 for harmonic oscillator.

## Physical Meaning

**V(x) = V(-x)** means potential has **inversion symmetry** - looks same from both sides of origin.

Examples:
- ✓ Harmonic oscillator: x²
- ✓ Even powers: x⁴, x⁶
- ✗ Odd powers: x, x³ (breaks symmetry)
- ✗ Linear potential: mgx (gravity)

## Consequence: Simultaneous Eigenstates

When [Π̂, Ĥ] = 0, they share eigenstates ([[Compatible and Incompatible Observables]]).

**Meaning**: Energy eigenstates |n⟩ automatically have definite parity.

For harmonic oscillator:
- Even n: even parity (+1)
- Odd n: odd parity (-1)

## Why This Matters

**Without symmetry analysis**:
1. Solve difficult differential equation
2. Get solutions ψₙ(x)
3. Notice "oh, they're even or odd"

**With symmetry analysis**:
1. Observe V(-x) = V(x)
2. Conclude [Π̂, Ĥ] = 0
3. Know solutions MUST be even or odd before solving
4. Can restrict search to even/odd functions only

**This simplifies solving** and reveals deep structure. Essential for 3D problems where symmetries (rotation, reflection) drastically constrain solutions.

## Related
- Previous: [[Parity Operator Action]]
- General principle: [[Compatible and Incompatible Observables]]
- Used in: [[Week 11.2 - Position Space Solution and Parity]]