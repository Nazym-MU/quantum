Derivation of excited state wave functions ⟨x|n⟩ for the [[Harmonic Oscillator]].
## Method: Apply Raising Operator
From [[Excited State Generation]]:
$$|n\rangle = \frac{(\hat{a}^\dagger)^n}{\sqrt{n!}}|0\rangle$$
Project to position space:
$$\langle x|n\rangle = \frac{1}{\sqrt{n!}}\langle x|(\hat{a}^\dagger)^n|0\rangle$$
## Raising Operator in Position Space
From [[Ladder Operators]]:
$$\hat{a}^\dagger = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} - \frac{i}{m\omega}\hat{p}_x\right)$$
In position representation:
$$\langle x|\hat{a}^\dagger = \sqrt{\frac{m\omega}{2\hbar}}\left(x - \frac{\hbar}{m\omega}\frac{\partial}{\partial x}\right)\langle x|$$

Therefore:
$$\langle x|\hat{a}^\dagger|\psi\rangle = \sqrt{\frac{m\omega}{2\hbar}}\left(x - \frac{\hbar}{m\omega}\frac{\partial}{\partial x}\right)\langle x|\psi\rangle$$

## General Formula

Define the position-space differential operator:
$$\hat{a}^\dagger_{\text{pos}} = \sqrt{\frac{m\omega}{2\hbar}}\left(x - \frac{\hbar}{m\omega}\frac{d}{dx}\right)$$

Then:
$$\langle x|n\rangle = \frac{1}{\sqrt{n!}}\left[\hat{a}^\dagger_{\text{pos}}\right]^n\langle x|0\rangle$$

With ⟨x|0⟩ from [[Ground State Wave Function Derivation]]:
$$\langle x|n\rangle = \frac{1}{\sqrt{n!}}\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}\left[\sqrt{\frac{m\omega}{2\hbar}}\left(x - \frac{\hbar}{m\omega}\frac{d}{dx}\right)\right]^n\exp\left(-\frac{m\omega x^2}{2\hbar}\right)$$

## Example: First Excited State |1⟩

$$\langle x|1\rangle = \sqrt{\frac{m\omega}{2\hbar}}\left(x - \frac{\hbar}{m\omega}\frac{d}{dx}\right)\langle x|0\rangle$$

Apply to ground state:
$$\frac{d}{dx}\left[e^{-m\omega x^2/2\hbar}\right] = -\frac{m\omega x}{\hbar}e^{-m\omega x^2/2\hbar}$$

Therefore:
$$\langle x|1\rangle = \sqrt{\frac{m\omega}{2\hbar}}\left[x + \frac{\hbar}{m\omega}\cdot\frac{m\omega x}{\hbar}\right]\langle x|0\rangle$$

$$= \sqrt{\frac{m\omega}{2\hbar}}\cdot 2x\langle x|0\rangle$$

$$= \sqrt{\frac{2m\omega}{\hbar}}x\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}e^{-m\omega x^2/2\hbar}$$

## Example: Second Excited State |2⟩

$$\langle x|2\rangle = \frac{1}{\sqrt{2}}\left[\hat{a}^\dagger_{\text{pos}}\right]^2\langle x|0\rangle$$

Apply operator twice (calculations omitted):
$$\langle x|2\rangle = \frac{1}{\sqrt{2}}\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}\left(\frac{2m\omega}{\hbar}x^2 - 1\right)e^{-m\omega x^2/2\hbar}$$

## Node Structure

The eigenfunction ⟨x|n⟩ has exactly **n nodes** (zeros where wave function crosses zero).
This follows from the polynomial factor of degree n that appears when applying (â†)^n.

## Connection to Hermite Polynomials

The wave functions can be written as:
$$\langle x|n\rangle = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4}\frac{1}{\sqrt{2^n n!}}H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)e^{-m\omega x^2/2\hbar}$$

where H_n are Hermite polynomials.

## Related

- [[Harmonic Oscillator Wave Functions]]
- [[Ground State Wave Function Derivation]]
- [[Ladder Operators]]
- [[Node Structure in Energy Eigenstates]]