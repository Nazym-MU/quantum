Detailed derivation of the [[Harmonic Oscillator]] ground state wave function ⟨x|0⟩.
## Starting Point
The ground state satisfies:
$$\hat{a}|0\rangle = 0$$
## Project to Position Space
Apply ⟨x| to both sides:
$$\langle x|\hat{a}|0\rangle = 0$$
## Substitute Ladder Operator
From [[Ladder Operators]]:
$$\hat{a} = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)$$

Therefore:
$$\langle x|\sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)|0\rangle = 0$$

$$\sqrt{\frac{m\omega}{2\hbar}}\left[\langle x|\hat{x}|0\rangle + \frac{i}{m\omega}\langle x|\hat{p}_x|0\rangle\right] = 0$$

## Apply Operators in Position Space

**Position operator**: x̂ acts on position eigenbra as eigenvalue
$$\langle x|\hat{x}|0\rangle = x\langle x|0\rangle$$

**Momentum operator**: From [[Momentum Operator in Position Basis]]:
$$\langle x|\hat{p}_x|0\rangle = \frac{\hbar}{i}\frac{\partial}{\partial x}\langle x|0\rangle$$

## Resulting Differential Equation

$$\sqrt{\frac{m\omega}{2\hbar}}\left[x\langle x|0\rangle + \frac{i}{m\omega}\cdot\frac{\hbar}{i}\frac{\partial}{\partial x}\langle x|0\rangle\right] = 0$$

$$x\langle x|0\rangle + \frac{\hbar}{m\omega}\frac{\partial}{\partial x}\langle x|0\rangle = 0$$

Rearranging:
$$\frac{\partial\langle x|0\rangle}{\partial x} = -\frac{m\omega}{\hbar}x\langle x|0\rangle$$

## Solve Differential Equation

This is separable:
$$\frac{d\psi_0}{\psi_0} = -\frac{m\omega}{\hbar}x\,dx$$

Integrate:
$$\ln|\psi_0| = -\frac{m\omega}{2\hbar}x^2 + C$$

$$\psi_0(x) = A\exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$

where A = e^C is the normalization constant.

## Normalization

Require:
$$\int_{-\infty}^{\infty}|\psi_0(x)|^2\,dx = 1$$

$$|A|^2\int_{-\infty}^{\infty}\exp\left(-\frac{m\omega x^2}{\hbar}\right)dx = 1$$

Use Gaussian integral: $\int_{-\infty}^{\infty}e^{-\alpha x^2}dx = \sqrt{\pi/\alpha}$

With α = mω/ℏ:
$$|A|^2\sqrt{\frac{\pi\hbar}{m\omega}} = 1$$

$$|A| = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4}$$

## Final Result

$$\langle x|0\rangle = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4}\exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$

This is a [[Gaussian Wave Packet]] centered at x = 0 with width parameter √(ℏ/mω).

## Related

- [[Harmonic Oscillator Wave Functions]]
- [[Ladder Operators]]
- [[Momentum Operator in Position Basis]]
- [[Zero-Point Energy]]