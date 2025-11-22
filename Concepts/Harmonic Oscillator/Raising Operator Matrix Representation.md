# Raising Operator Matrix Representation

The matrix representation of the raising operator â† in the energy eigenbasis {|n⟩}.

## Matrix Form

$$\hat{a}^\dagger \to \begin{pmatrix} 0 & 0 & 0 & 0 & \cdots \\ \sqrt{1} & 0 & 0 & 0 & \cdots \\ 0 & \sqrt{2} & 0 & 0 & \cdots \\ 0 & 0 & \sqrt{3} & 0 & \cdots \\ \vdots & \vdots & \vdots & \vdots & \ddots \end{pmatrix}$$

## Matrix Elements

The matrix elements are:
$$\langle n'|\hat{a}^\dagger|n\rangle = \sqrt{n+1}\,\delta_{n',n+1}$$

Derivation: [[Raising Operator Matrix Elements]]

**Interpretation**: Matrix element is non-zero only when n' = n + 1, reflecting that â† raises the quantum number by 1.

## Structure

**Non-diagonal**: The matrix has non-zero elements only on the superdiagonal (one position above the main diagonal).

**Why non-diagonal?** See: [[Why Ladder Operators Are Not Diagonal]]

If â† were diagonal, it would share eigenstates with Ĥ. But â†|n⟩ = √(n+1)|n+1⟩ ≠ λ|n⟩, so |n⟩ is not an eigenstate of â†.

## Connection to Position and Momentum

Using the inverse relations from [[Ladder Operators]]:
$$\hat{x} = \sqrt{\frac{\hbar}{2m\omega}}(\hat{a} + \hat{a}^\dagger)$$
$$\hat{p}_x = i\sqrt{\frac{m\hbar\omega}{2}}(\hat{a}^\dagger - \hat{a})$$

The matrix representations of x̂ and p̂ₓ can be constructed from â and â†.

## Related Concepts

- [[Ladder Operators]]
- [[Lowering Operator Matrix Representation]]
- [[Matrix Representations]]
- [[Why Ladder Operators Are Not Diagonal]]