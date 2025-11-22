Explanation of why [[Ladder Operators]] â and â† have non-diagonal matrix representations in the energy eigenbasis.
## Eigenstate Condition
An operator Ô is diagonal in a basis {|n⟩} if and only if the basis states are eigenstates of Ô:
$$\hat{O}|n\rangle = \lambda_n|n\rangle$$
The matrix elements would then be:
$$\langle n'|\hat{O}|n\rangle = \lambda_n \delta_{n',n}$$

## Ladder Operator Actions
The [[Harmonic Oscillator]] energy eigenstates |n⟩ satisfy:
$$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle \neq \lambda|n\rangle$$
$$\hat{a}|n\rangle = \sqrt{n}|n-1\rangle \neq \lambda|n\rangle$$

Since â†|n⟩ and â|n⟩ are **different states** (not proportional to |n⟩), the states |n⟩ are not eigenstates of the ladder operators.

## Physical Interpretation

The ladder operators **change** the quantum state by adding or removing one quantum of energy:
- â† raises energy: En → En+1
- â lowers energy: En → En-1

If they were diagonal, they would leave the state unchanged (except for a phase), which contradicts their defining property.

## Diagonal Operators

In contrast, the [[Number Operator]] N̂ = â†â **is diagonal** because:
$$\hat{N}|n\rangle = n|n\rangle$$

The states |n⟩ are eigenstates of N̂, so:
$$\langle n'|\hat{N}|n\rangle = n\delta_{n',n}$$

The [[Hamiltonian Operator|Hamiltonian]] Ĥ = ℏω(N̂ + ½) is also diagonal in this basis.

## Matrix Structure

Since â†|n⟩ = √(n+1)|n+1⟩:
$$\langle n'|\hat{a}^\dagger|n\rangle = \sqrt{n+1}\langle n'|n+1\rangle = \sqrt{n+1}\delta_{n',n+1}$$

This gives non-zero elements only on the **superdiagonal** (see [[Raising Operator Matrix Representation]]).

Similarly, â has non-zero elements only on the **subdiagonal** (see [[Lowering Operator Matrix Representation]]).

## Related Concepts

- [[Ladder Operators]]
- [[Raising Operator Matrix Representation]]
- [[Lowering Operator Matrix Representation]]
- [[Number Operator]]
- [[Matrix Representations]]
- [[Diagonalization]]