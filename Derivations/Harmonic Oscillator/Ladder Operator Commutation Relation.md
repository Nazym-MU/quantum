Derivation of [â, â†] = 1 for [[Harmonic Oscillator]] [[Ladder Operators]].
## Given

$$\hat{a} = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)$$
$$\hat{a}^\dagger = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} - \frac{i}{m\omega}\hat{p}_x\right)$$
Fundamental commutator: \[x̂, p̂ₓ\] = iℏ (see [[Position-Momentum Commutator]])
## Derivation
Compute the commutator:
$$[\hat{a}, \hat{a}^\dagger] = \hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a}$$

Substitute definitions:
$$[\hat{a}, \hat{a}^\dagger] = \frac{m\omega}{2\hbar}\left[\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)\left(\hat{x} - \frac{i}{m\omega}\hat{p}_x\right) - \left(\hat{x} - \frac{i}{m\omega}\hat{p}_x\right)\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)\right]$$

Expand the products:
$$\hat{a}\hat{a}^\dagger = \frac{m\omega}{2\hbar}\left(\hat{x}^2 - \frac{i}{m\omega}\hat{x}\hat{p}_x + \frac{i}{m\omega}\hat{p}_x\hat{x} + \frac{1}{m^2\omega^2}\hat{p}_x^2\right)$$

$$\hat{a}^\dagger\hat{a} = \frac{m\omega}{2\hbar}\left(\hat{x}^2 + \frac{i}{m\omega}\hat{x}\hat{p}_x - \frac{i}{m\omega}\hat{p}_x\hat{x} + \frac{1}{m^2\omega^2}\hat{p}_x^2\right)$$

Take the difference (x̂² and p̂ₓ² terms cancel):
$$[\hat{a}, \hat{a}^\dagger] = \frac{m\omega}{2\hbar} \cdot \frac{2i}{m\omega}(\hat{p}_x\hat{x} - \hat{x}\hat{p}_x)$$

$$= \frac{i}{\hbar}(-[\hat{x}, \hat{p}_x])$$

$$= \frac{i}{\hbar}(-i\hbar)$$

$$= 1$$

## Result

$$[\hat{a}, \hat{a}^\dagger] = 1$$

This fundamental commutator drives all properties of the harmonic oscillator.

## Consequences

From this commutator:
- [[Number Operator]] commutators: $[\hat{N}, â]=-\hat{a}$ and $[\hat{N}, â^\dagger]=\hat{a}^\dagger$
- Matrix elements: [[Raising Operator Matrix Elements]], [[Lowering Operator Matrix Elements]]
- Energy spectrum quantization

## Related

- [[Ladder Operators]]
- [[Position-Momentum Commutator]]
- [[Hamiltonian in Terms of Number Operator]]