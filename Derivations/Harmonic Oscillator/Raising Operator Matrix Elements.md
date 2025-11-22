Derivation of $⟨n'|â†|n⟩ = \sqrt{(n+1)}δ_{n', n+1}$ for the [[Harmonic Oscillator]].
## Goal
Find the matrix elements of the raising operator â† in the energy eigenbasis.
## Step 1: Action of â†
From [[Number Operator Eigenvalue Derivation]], we know:
$$\hat{N}\hat{a}^\dagger|n\rangle = (n+1)\hat{a}^\dagger|n\rangle$$
This means â†|n⟩ is an eigenstate of N̂ with eigenvalue n+1:
$$\hat{a}^\dagger|n\rangle = c_n|n+1\rangle$$
where cₙ is a constant to be determined.
## Step 2: Determine Normalization Constant
Take the inner product:
$$\langle n|\hat{a}\hat{a}^\dagger|n\rangle = |c_n|^2\langle n+1|n+1\rangle = |c_n|^2$$
(assuming normalized states)
## Step 3: Use Commutation Relation
From [[Ladder Operator Commutation Relation]]:
$$[\hat{a}, \hat{a}^\dagger] = \hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a} = 1$$

Therefore:
$$\hat{a}\hat{a}^\dagger = \hat{a}^\dagger\hat{a} + 1 = \hat{N} + 1$$

## Step 4: Evaluate

$$\langle n|\hat{a}\hat{a}^\dagger|n\rangle = \langle n|(\hat{N} + 1)|n\rangle = (n+1)\langle n|n\rangle = n+1$$

## Step 5: Solve for Constant

From steps 2 and 4:
$$|c_n|^2 = n+1$$

Choose phase convention: cₙ = √(n+1) (real and positive)

Therefore:
$$\boxed{\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle}$$

## Matrix Element Formula

Taking the inner product with ⟨n'|:
$$\langle n'|\hat{a}^\dagger|n\rangle = \sqrt{n+1}\langle n'|n+1\rangle = \sqrt{n+1}\delta_{n',n+1}$$

## Matrix Representation

The matrix of â† in the {|0⟩, |1⟩, |2⟩, ...} basis is:

$$\hat{a}^\dagger \to \begin{pmatrix}
0 & 0 & 0 & 0 & \cdots \\
\sqrt{1} & 0 & 0 & 0 & \cdots \\
0 & \sqrt{2} & 0 & 0 & \cdots \\
0 & 0 & \sqrt{3} & 0 & \cdots \\
\vdots & \vdots & \vdots & \vdots & \ddots
\end{pmatrix}$$

Elements: $(a^\dagger)_{ij} = \langle i|\hat{a}^\dagger|j\rangle = \sqrt{j+1}\delta_{i,j+1}$

## Why Non-Diagonal?

The raising operator connects different energy eigenstates:
- Takes |n⟩ → |n+1⟩
- Increases energy by ℏω
- **Cannot be diagonal** in energy eigenbasis

If it were diagonal:
- Would commute with Ĥ
- Would preserve energy (contradiction!)

## Physical Interpretation

The matrix element √(n+1) grows with n because:
1. Higher states have more "room" for additional quanta
2. Bosonic enhancement: easier to add particles to occupied states
3. Normalization requirement from multiple application

## Connection to Creation Operator

In quantum field theory context (photons):
- â†|n⟩ = √(n+1)|n+1⟩ creates a photon
- Probability amplitude ∝ √(n+1)
- Probability ∝ (n+1): stimulated emission enhancement

## Related

- [[Lowering Operator Matrix Elements]]
- [[Ladder Operators]]
- [[Number Operator Eigenvalue Derivation]]
- [[Why Ladder Operators Are Not Diagonal]]
- [[Excited State Generation]]