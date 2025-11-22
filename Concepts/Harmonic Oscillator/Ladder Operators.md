Non-Hermitian operators for the [[Harmonic Oscillator]] that raise or lower the energy eigenstate by one quantum.
**Lowering operator** (annihilation operator):
$$\hat{a} = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} + \frac{i}{m\omega}\hat{p}_x\right)$$
**Raising operator** (creation operator):
$$\hat{a}^\dagger = \sqrt{\frac{m\omega}{2\hbar}}\left(\hat{x} - \frac{i}{m\omega}\hat{p}_x\right)$$
The $\sqrt{(mω/2ℏ)}$ factor makes them dimensionless.

## Commutation Relation

$$[\hat{a}, \hat{a}^\dagger] = 1$$
Derivation: [[Ladder Operator Commutation Relation]]
This follows from [[Position-Momentum Commutator]] [x̂,p̂ₓ] = iℏ.

## Actions on States

$$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$$
$$\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$$

Derivations: [[Raising Operator Matrix Elements]], [[Lowering Operator Matrix Elements]]
The ground state satisfies:
$$\hat{a}|0\rangle = 0$$
## Matrix Representations
In the energy eigenbasis {|n⟩}, the operators have matrix representations:

$$\hat{a}^\dagger \to \begin{pmatrix} 0 & 0 & 0 & \cdots \\ \sqrt{1} & 0 & 0 & \cdots \\ 0 & \sqrt{2} & 0 & \cdots \\ 0 & 0 & \sqrt{3} & \cdots \\ \vdots & \vdots & \vdots & \ddots \end{pmatrix} \qquad \hat{a} \to \begin{pmatrix} 0 & \sqrt{1} & 0 & 0 & \cdots \\ 0 & 0 & \sqrt{2} & 0 & \cdots \\ 0 & 0 & 0 & \sqrt{3} & \cdots \\ \vdots & \vdots & \vdots & \vdots & \ddots \end{pmatrix}$$
See: [[Why Ladder Operators Are Not Diagonal]]

## Physical Interpretation

In quantum field theory (photons, phonons):
- â† creates one quantum of excitation (creation operator)
- â destroys one quantum (annihilation operator)
- The number of quanta is n (number operator eigenvalue)

## Inverse Relations

Position and momentum operators in terms of ladder operators:
$$\hat{x} = \sqrt{\frac{\hbar}{2m\omega}}(\hat{a} + \hat{a}^\dagger)$$
$$\hat{p}_x = i\sqrt{\frac{m\hbar\omega}{2}}(\hat{a}^\dagger - \hat{a})$$

## Related Concepts
- [[Number Operator]]: N̂ = â†â
- [[Harmonic Oscillator]]
- [[Raising and Lowering Operators]] (angular momentum analogy)
- [[Raising Operator Matrix Representation]]
- [[Lowering Operator Matrix Representation]]