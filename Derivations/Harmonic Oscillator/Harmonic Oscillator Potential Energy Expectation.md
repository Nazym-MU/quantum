# Harmonic Oscillator Potential Energy Expectation

Derivation of ⟨V⟩ₙ = ⟨½mω²x²⟩ₙ for [[Harmonic Oscillator]] energy eigenstates.

## Setup

The potential energy operator is:
$$\hat{V} = \frac{1}{2}m\omega^2\hat{x}^2$$

We need to evaluate:
$$\langle V\rangle_n = \langle n|\frac{1}{2}m\omega^2\hat{x}^2|n\rangle$$

## Express x̂ in Terms of Ladder Operators

From [[Ladder Operators]]:
$$\hat{x} = \sqrt{\frac{\hbar}{2m\omega}}(\hat{a} + \hat{a}^\dagger)$$

Therefore:
$$\hat{x}^2 = \frac{\hbar}{2m\omega}(\hat{a} + \hat{a}^\dagger)^2$$

## Expand the Square

$$(\hat{a} + \hat{a}^\dagger)^2 = \hat{a}^2 + \hat{a}\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + (\hat{a}^\dagger)^2$$

## Use Commutation Relation

From [[Ladder Operator Commutation Relation]]: [â, â†] = 1

This gives: ââ† = â†â + 1 = N̂ + 1

Substitute:
$$(\hat{a} + \hat{a}^\dagger)^2 = \hat{a}^2 + (\hat{N} + 1) + \hat{N} + (\hat{a}^\dagger)^2$$

$$= \hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1$$

where N̂ = â†â is the [[Number Operator]].

## Calculate x̂²

$$\hat{x}^2 = \frac{\hbar}{2m\omega}(\hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1)$$

## Potential Energy Operator

$$\hat{V} = \frac{1}{2}m\omega^2 \cdot \frac{\hbar}{2m\omega}(\hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1)$$

$$= \frac{\hbar\omega}{4}(\hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1)$$

## Evaluate Expectation Value

$$\langle n|\hat{V}|n\rangle = \frac{\hbar\omega}{4}\langle n|(\hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1)|n\rangle$$

Using [[Raising Operator Matrix Elements]] and [[Lowering Operator Matrix Elements]]:

**Term 1**: 
$$\langle n|\hat{a}^2|n\rangle = \sqrt{n(n-1)}\langle n|n-2\rangle = 0$$
(orthogonality of eigenstates)

**Term 2**: 
$$\langle n|(\hat{a}^\dagger)^2|n\rangle = \sqrt{(n+1)(n+2)}\langle n|n+2\rangle = 0$$
(orthogonality)

**Term 3**: ⟨n|2N̂|n⟩ = 2n

**Term 4**: ⟨n|1|n⟩ = 1

Therefore:
$$\langle V\rangle_n = \frac{\hbar\omega}{4}(0 + 0 + 2n + 1)$$

$$\boxed{\langle V\rangle_n = \frac{\hbar\omega}{4}(2n+1)}$$

## Alternative Form

$$\langle V\rangle_n = \frac{\hbar\omega}{2}\left(n + \frac{1}{2}\right)$$

## Special Cases

**Ground state (n=0)**:
$$\langle V\rangle_0 = \frac{\hbar\omega}{4}$$

**First excited state (n=1)**:
$$\langle V\rangle_1 = \frac{3\hbar\omega}{4}$$

## Comparison with Total Energy

From [[Hamiltonian in Terms of Number Operator]]:
$$E_n = \hbar\omega\left(n + \frac{1}{2}\right)$$

Therefore:
$$\frac{\langle V\rangle_n}{E_n} = \frac{1}{2}$$

**The potential energy is exactly half the total energy**, regardless of n.

## Virial Theorem

For the harmonic oscillator:
$$\langle T\rangle_n = \langle V\rangle_n = \frac{E_n}{2}$$

This is a specific case of the virial theorem. See [[Harmonic Oscillator Kinetic Energy Expectation]].

**Energy partition**:
- Kinetic: E_n/2
- Potential: E_n/2
- Total: E_n = ℏω(n + 1/2)

## Physical Interpretation

The equal partition of energy between kinetic and potential forms is characteristic of the harmonic oscillator.

As n increases:
- More spatial extent: ⟨x²⟩ ∝ (2n+1) (see [[Harmonic Oscillator Position Uncertainty]])
- Wave function spreads to regions of higher potential
- But maintains 50-50 energy split

## Connection to Classical Oscillator

Classically, for a particle oscillating with amplitude A:
- At turning points: All potential energy = ½mω²A²
- At equilibrium: All kinetic energy = ½m(ωA)²
- Time average: ⟨T⟩ = ⟨V⟩ = E/2

The quantum result matches the classical time average, reflecting the correspondence principle.

## Related

- [[Harmonic Oscillator Kinetic Energy Expectation]]
- [[Harmonic Oscillator Position Uncertainty]]
- [[Ladder Operators]]
- [[Classical Turning Points]]