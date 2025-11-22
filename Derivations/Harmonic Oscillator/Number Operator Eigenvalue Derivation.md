# Number Operator Eigenvalue Derivation

Derivation showing that [[Number Operator]] N̂ has non-negative integer eigenvalues.

## Setup

Define N̂ = â†â where â, â† are [[Ladder Operators]] with [â, â†] = 1.

Let |η⟩ be an eigenstate: N̂|η⟩ = η|η⟩

## Non-Negativity

Compute the expectation value in state |η⟩:
$$\langle \eta|\hat{N}|\eta\rangle = \langle \eta|\hat{a}^\dagger\hat{a}|\eta\rangle = \eta\langle\eta|\eta\rangle = \eta$$

Define |ψ⟩ = â|η⟩. Then:
$$\langle \eta|\hat{a}^\dagger\hat{a}|\eta\rangle = \langle\psi|\psi\rangle \geq 0$$

Since ⟨ψ|ψ⟩ is a norm squared (always ≥ 0) and equals η:
$$\eta \geq 0$$

Therefore eigenvalues of N̂ are **non-negative**.

## Commutators with Ladder Operators

Using [â, â†] = 1, compute:

$$[\hat{N}, \hat{a}] = [\hat{a}^\dagger\hat{a}, \hat{a}] = \hat{a}^\dagger[\hat{a}, \hat{a}] + [\hat{a}^\dagger, \hat{a}]\hat{a}$$

Since [â, â] = 0 and [â†, â] = -[â, â†] = -1:
$$[\hat{N}, \hat{a}] = -\hat{a}$$

Similarly:
$$[\hat{N}, \hat{a}^\dagger] = \hat{a}^\dagger$$

## Action of Lowering Operator

Apply N̂ to â|η⟩:
$$\hat{N}\hat{a}|\eta\rangle = (\hat{a}\hat{N} - \hat{a})|\eta\rangle = \hat{a}(\hat{N} - 1)|\eta\rangle = (η - 1)\hat{a}|\eta\rangle$$

Therefore â|η⟩ is an eigenstate of N̂ with eigenvalue (η - 1).

Similarly, â†|η⟩ has eigenvalue (η + 1).

## Ladder Must Terminate

Starting from |η⟩, repeatedly applying â generates states with eigenvalues:
$$\eta, \eta-1, \eta-2, \eta-3, \ldots$$

Since eigenvalues must be non-negative, this sequence must terminate. There must exist a minimum eigenvalue ηₘᵢₙ such that:
$$\hat{a}|\eta_{\min}\rangle = 0$$

## Determining Minimum Value

If â|ηₘᵢₙ⟩ = 0, then:
$$\hat{N}|\eta_{\min}\rangle = \hat{a}^\dagger\hat{a}|\eta_{\min}\rangle = \hat{a}^\dagger \cdot 0 = 0$$

Therefore ηₘᵢₙ = 0.

Applying â† repeatedly to |0⟩ generates:
$$\hat{a}^\dagger|0\rangle = c_1|1\rangle$$
$$(\hat{a}^\dagger)^2|0\rangle = c_2|2\rangle$$
$$(\hat{a}^\dagger)^n|0\rangle = c_n|n\rangle$$

with eigenvalues 0, 1, 2, 3, ...

## Result

The eigenvalues of N̂ are:
$$\eta = n = 0, 1, 2, 3, \ldots$$

The eigenstates are labeled |n⟩ with:
$$\hat{N}|n\rangle = n|n\rangle$$

## Energy Spectrum

Since Ĥ = ℏω(N̂ + ½), the energy eigenvalues are:
$$E_n = \hbar\omega\left(n + \frac{1}{2}\right)$$

See: [[Hamiltonian in Terms of Number Operator]]

## Related

- [[Number Operator]]
- [[Ladder Operators]]
- [[Ladder Operator Commutation Relation]]
- [[Why Lambda Non-negative]] (similar proof for angular momentum)