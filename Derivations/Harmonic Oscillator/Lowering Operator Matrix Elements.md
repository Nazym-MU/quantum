Derivation of ⟨n'|â|n⟩ = √n δₙ',ₙ₋₁ for the [[Harmonic Oscillator]].
## Goal
Find the matrix elements of the lowering operator â in the energy eigenbasis.
## Step 1: Action of â
From [[Number Operator Eigenvalue Derivation]], we know:
$$\hat{N}\hat{a}|n\rangle = (n-1)\hat{a}|n\rangle$$

This means â|n⟩ is an eigenstate of $\hat{N}$ with eigenvalue n-1:
$$\hat{a}|n\rangle = d_n|n-1\rangle$$

where dₙ is a constant to be determined.

## Step 2: Determine Normalization Constant

Take the inner product:
$$\langle n|\hat{a}^\dagger\hat{a}|n\rangle = |d_n|^2\langle n-1|n-1\rangle = |d_n|^2$$

(assuming normalized states)

## Step 3: Use Number Operator

The number operator is defined as:
$$\hat{N} = \hat{a}^\dagger\hat{a}$$

With N̂|n⟩ = n|n⟩ from [[Number Operator Eigenvalue Derivation]].

## Step 4: Evaluate

$$\langle n|\hat{a}^\dagger\hat{a}|n\rangle = \langle n|\hat{N}|n\rangle = n\langle n|n\rangle = n$$

## Step 5: Solve for Constant

From steps 2 and 4:
$$|d_n|^2 = n$$

Choose phase convention: dₙ = √n (real and positive)

Therefore:
$$\boxed{\hat{a}|n\rangle = \sqrt{n}|n-1\rangle}$$

## Ground State

For n = 0:
$$\hat{a}|0\rangle = \sqrt{0}|{-1}\rangle = 0$$

The ground state is **annihilated** by â, which is why â|0⟩ = 0 is used to find the ground state wave function (see [[Ground State Wave Function Derivation]]).

## Matrix Element Formula

Taking the inner product with ⟨n'|:
$$\langle n'|\hat{a}|n\rangle = \sqrt{n}\langle n'|n-1\rangle = \sqrt{n}\delta_{n',n-1}$$

## Matrix Representation

The matrix of â in the {|0⟩, |1⟩, |2⟩, ...} basis is:

$$\hat{a} \to \begin{pmatrix}
0 & \sqrt{1} & 0 & 0 & \cdots \\
0 & 0 & \sqrt{2} & 0 & \cdots \\
0 & 0 & 0 & \sqrt{3} & \cdots \\
0 & 0 & 0 & 0 & \cdots \\
\vdots & \vdots & \vdots & \vdots & \ddots
\end{pmatrix}$$

Elements: $(a)_{ij} = \langle i|\hat{a}|j\rangle = \sqrt{j}\delta_{i,j-1}$

## Relationship to â†

The matrices are related by:
$$\hat{a} = (\hat{a}^\dagger)^\dagger$$

In matrix form: $a = (a^\dagger)^T$ (transpose, since operators are Hermitian adjoints)

Compare with [[Raising Operator Matrix Elements]]:
- â† has non-zero elements on **super-diagonal** (above main diagonal)
- â has non-zero elements on **sub-diagonal** (below main diagonal)

## Why Non-Diagonal?

The lowering operator connects different energy eigenstates:
- Takes |n⟩ → |n-1⟩
- Decreases energy by ℏω
- **Cannot be diagonal** in energy eigenbasis

If it were diagonal:
- Would commute with Ĥ
- Would preserve energy (contradiction!)

See [[Why Ladder Operators Are Not Diagonal]] for detailed explanation.

## Physical Interpretation

The matrix element √n shrinks as n decreases because:
1. Fewer quanta available to remove
2. Ground state (n=0) cannot be lowered further
3. Normalization requirement

## Connection to Annihilation Operator

In quantum field theory context (photons):
- â|n⟩ = √n|n-1⟩ destroys a photon
- Probability amplitude ∝ √n
- Probability ∝ n: proportional to number of photons present

## Verification of Commutation Relation

Using the matrix representations:
$$[\hat{a}, \hat{a}^\dagger]_{ij} = \sum_k (a_{ik}a^\dagger_{kj} - a^\dagger_{ik}a_{kj})$$

$$= \sqrt{i}\delta_{i,k-1}\sqrt{k+1}\delta_{k+1,j} - \sqrt{k+1}\delta_{i,k+1}\sqrt{j}\delta_{k,j-1}$$

After working through the algebra (i = j case):
$$= \delta_{ij}$$

Confirming [â, â†] = 1. ✓

## Related

- [[Raising Operator Matrix Elements]]
- [[Ladder Operators]]
- [[Number Operator Eigenvalue Derivation]]
- [[Ground State Wave Function Derivation]]
- [[Why Ladder Operators Are Not Diagonal]]