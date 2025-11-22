# Harmonic Oscillator Kinetic Energy Expectation

Derivation of ⟨T⟩ₙ = ⟨p̂²/2m⟩ₙ for [[Harmonic Oscillator]] energy eigenstates.

## Setup

The kinetic energy operator is:
$$\hat{T} = \frac{\hat{p}_x^2}{2m}$$

We need to evaluate:
$$\langle T\rangle_n = \langle n|\frac{\hat{p}_x^2}{2m}|n\rangle$$

## Express p̂ₓ in Terms of Ladder Operators

From [[Ladder Operators]]:
$$\hat{p}_x = -i\sqrt{\frac{m\omega\hbar}{2}}(\hat{a} - \hat{a}^\dagger)$$

Therefore:
$$\hat{p}_x^2 = -\frac{m\omega\hbar}{2}(\hat{a} - \hat{a}^\dagger)^2$$

## Expand the Square

$$(\hat{a} - \hat{a}^\dagger)^2 = \hat{a}^2 - \hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a} + (\hat{a}^\dagger)^2$$

## Use Commutation Relation

From [[Ladder Operator Commutation Relation]]: [â, â†] = 1

This gives: ââ† = â†â + 1

Substitute:
$$(\hat{a} - \hat{a}^\dagger)^2 = \hat{a}^2 - (\hat{a}^\dagger\hat{a} + 1) - \hat{a}^\dagger\hat{a} + (\hat{a}^\dagger)^2$$

$$= \hat{a}^2 + (\hat{a}^\dagger)^2 - 2\hat{a}^\dagger\hat{a} - 1$$

$$= \hat{a}^2 + (\hat{a}^\dagger)^2 - 2\hat{N} - 1$$

where N̂ = â†â is the [[Number Operator]].

## Calculate p̂ₓ²

$$\hat{p}_x^2 = -\frac{m\omega\hbar}{2}(\hat{a}^2 + (\hat{a}^\dagger)^2 - 2\hat{N} - 1)$$

$$= \frac{m\omega\hbar}{2}(2\hat{N} + 1 - \hat{a}^2 - (\hat{a}^\dagger)^2)$$

## Evaluate Expectation Value

$$\langle n|\hat{p}_x^2|n\rangle = \frac{m\omega\hbar}{2}\langle n|(2\hat{N} + 1 - \hat{a}^2 - (\hat{a}^\dagger)^2)|n\rangle$$

Using [[Raising Operator Matrix Elements]] and [[Lowering Operator Matrix Elements]]:

**Term 1**: ⟨n|2N̂|n⟩ = 2n

**Term 2**: ⟨n|1|n⟩ = 1

**Term 3**: 
$$\langle n|\hat{a}^2|n\rangle = \sqrt{n(n-1)}\langle n|n-2\rangle = 0$$
(orthogonality)

**Term 4**: 
$$\langle n|(\hat{a}^\dagger)^2|n\rangle = \sqrt{(n+1)(n+2)}\langle n|n+2\rangle = 0$$
(orthogonality)

Therefore:
$$\langle p_x^2\rangle_n = \frac{m\omega\hbar}{2}(2n + 1)$$

## Kinetic Energy

$$\langle T\rangle_n = \frac{\langle p_x^2\rangle_n}{2m} = \frac{m\omega\hbar(2n+1)}{2 \cdot 2m}$$

$$\boxed{\langle T\rangle_n = \frac{\hbar\omega}{4}(2n+1)}$$

## Alternative Form

$$\langle T\rangle_n = \frac{\hbar\omega}{2}\left(n + \frac{1}{2}\right)$$

## Special Cases

**Ground state (n=0)**:
$$\langle T\rangle_0 = \frac{\hbar\omega}{4}$$

**First excited state (n=1)**:
$$\langle T\rangle_1 = \frac{3\hbar\omega}{4}$$

## Comparison with Total Energy

From [[Hamiltonian in Terms of Number Operator]]:
$$E_n = \hbar\omega\left(n + \frac{1}{2}\right)$$

Therefore:
$$\frac{\langle T\rangle_n}{E_n} = \frac{1}{2}$$

**The kinetic energy is exactly half the total energy**, regardless of n.

## Connection to Potential Energy

By the virial theorem for harmonic oscillator:
$$\langle V\rangle_n = \langle T\rangle_n = \frac{E_n}{2}$$

See [[Harmonic Oscillator Potential Energy Expectation]] for detailed derivation.

## Physical Interpretation

As n increases:
- More quanta in the state
- Higher average momentum: ⟨p²⟩ ∝ (2n+1)
- More oscillatory wave function (see [[Node Structure in Energy Eigenstates]])
- Greater curvature in ⟨x|n⟩

The kinetic energy grows linearly with n because each quantum adds ℏω/2 to both kinetic and potential energy equally.

## Related

- [[Harmonic Oscillator Potential Energy Expectation]]
- [[Harmonic Oscillator Momentum Uncertainty]]
- [[Ladder Operators]]
- [[Expectation Values]]