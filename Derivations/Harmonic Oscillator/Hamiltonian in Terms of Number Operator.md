Derivation showing Ĥ = ℏω(N̂ + ½) for the [[Harmonic Oscillator]].
## Given
Hamiltonian:
$$\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2$$
[[Ladder Operators]]:
$$\hat{a} = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)$$
$$\hat{a}^\dagger = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} - \frac{i}{m\omega}\hat{p}_x\right)$$
## Inverse Relations

Solve for x̂ and p̂ₓ:

Add â and â†:
$$\hat{a} + \hat{a}^\dagger = \sqrt{\frac{m\omega}{2\hbar}} \cdot 2\hat{x}$$
$$\hat{x} = \sqrt{\frac{\hbar}{2m\omega}}(\hat{a} + \hat{a}^\dagger)$$

Subtract â from â†:
$$\hat{a}^\dagger - \hat{a} = \sqrt{\frac{m\omega}{2\hbar}} \cdot \left(-\frac{2i}{m\omega}\hat{p}_x\right)$$
$$\hat{p}_x = i\sqrt{\frac{m\hbar\omega}{2}}(\hat{a}^\dagger - \hat{a})$$

## Substitute into Hamiltonian

Compute p̂ₓ²:
$$\hat{p}_x^2 = -\frac{m\hbar\omega}{2}(\hat{a}^\dagger - \hat{a})^2 = -\frac{m\hbar\omega}{2}(\hat{a}^{\dagger 2} - \hat{a}^\dagger\hat{a} - \hat{a}\hat{a}^\dagger + \hat{a}^2)$$

Compute x̂²:
$$\hat{x}^2 = \frac{\hbar}{2m\omega}(\hat{a} + \hat{a}^\dagger)^2 = \frac{\hbar}{2m\omega}(\hat{a}^2 + \hat{a}\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + \hat{a}^{\dagger 2})$$

Kinetic energy:
$$\frac{\hat{p}^2}{2m} = -\frac{\hbar\omega}{4}(\hat{a}^{\dagger 2} - \hat{a}^\dagger\hat{a} - \hat{a}\hat{a}^\dagger + \hat{a}^2)$$

Potential energy:
$$\frac{1}{2}m\omega^2\hat{x}^2 = \frac{\hbar\omega}{4}(\hat{a}^2 + \hat{a}\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + \hat{a}^{\dagger 2})$$

## Add Terms

$$\hat{H} = \frac{\hbar\omega}{4}[-\hat{a}^{\dagger 2} + \hat{a}^\dagger\hat{a} + \hat{a}\hat{a}^\dagger - \hat{a}^2 + \hat{a}^2 + \hat{a}\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + \hat{a}^{\dagger 2}]$$

The â² and â†² terms cancel:
$$\hat{H} = \frac{\hbar\omega}{4}[2\hat{a}^\dagger\hat{a} + 2\hat{a}\hat{a}^\dagger]$$

$$= \frac{\hbar\omega}{2}(\hat{a}^\dagger\hat{a} + \hat{a}\hat{a}^\dagger)$$

## Use Commutation Relation

From [[Ladder Operator Commutation Relation]]: [â, â†] = ââ† - â†â = 1

Therefore: ââ† = â†â + 1

Substitute:
$$\hat{H} = \frac{\hbar\omega}{2}(\hat{a}^\dagger\hat{a} + \hat{a}^\dagger\hat{a} + 1)$$

$$= \hbar\omega\left(\hat{a}^\dagger\hat{a} + \frac{1}{2}\right)$$

## Final Result

Define [[Number Operator]] N̂ = â†â:

$$\hat{H} = \hbar\omega\left(\hat{N} + \frac{1}{2}\right)$$

This shows the energy eigenvalues are:
$$E_n = \hbar\omega\left(n + \frac{1}{2}\right)$$

where n are eigenvalues of N̂.

## Related

- [[Number Operator]]
- [[Ladder Operators]]
- [[Ladder Operator Commutation Relation]]
- [[Zero-Point Energy]]