# Lowering Operator Matrix Representation

The matrix representation of the lowering operator â in the energy eigenbasis {|n⟩}.

## Matrix Form

$$\hat{a} \to \begin{pmatrix} 0 & \sqrt{1} & 0 & 0 & \cdots \\ 0 & 0 & \sqrt{2} & 0 & \cdots \\ 0 & 0 & 0 & \sqrt{3} & \cdots \\ 0 & 0 & 0 & 0 & \cdots \\ \vdots & \vdots & \vdots & \vdots & \ddots \end{pmatrix}$$

## Matrix Elements

The matrix elements are:
$$\langle n'|\hat{a}|n\rangle = \sqrt{n}\,\delta_{n',n-1}$$

Derivation: [[Lowering Operator Matrix Elements]]

**Interpretation**: Matrix element is non-zero only when n' = n - 1, reflecting that â lowers the quantum number by 1.

## Structure

**Non-diagonal**: The matrix has non-zero elements only on the subdiagonal (one position below the main diagonal).

**Why non-diagonal?** See: [[Why Ladder Operators Are Not Diagonal]]

If â were diagonal, it would share eigenstates with Ĥ. But â|n⟩ = √n|n-1⟩ ≠ λ|n⟩, so |n⟩ is not an eigenstate of â.

## Relation to Raising Operator

The lowering operator is the adjoint of the raising operator:
$$\hat{a} = (\hat{a}^\dagger)^\dagger$$

Therefore, their matrix representations are related by Hermitian conjugation (transpose and complex conjugate):
$$[\hat{a}] = [\hat{a}^\dagger]^\dagger$$

## Number Operator

The [[Number Operator]] N̂ = â†â has matrix representation:
$$\hat{N} = \hat{a}^\dagger\hat{a} \to \begin{pmatrix} 0 & 0 & 0 & \cdots \\ 0 & 1 & 0 & \cdots \\ 0 & 0 & 2 & \cdots \\ \vdots & \vdots & \vdots & \ddots \end{pmatrix}$$

which is diagonal with eigenvalues n.

## Related Concepts

- [[Ladder Operators]]
- [[Raising Operator Matrix Representation]]
- [[Matrix Representations]]
- [[Why Ladder Operators Are Not Diagonal]]