Completely antisymmetric tensor εᵢⱼₖ used to express commutation relations and cross products.
### Properties:
- **Complete antisymmetry**: Interchanging any two indices changes the sign:
	- εᵢⱼₖ = -εⱼᵢₖ = -εᵢₖⱼ
- **Normalization**: ε₁₂₃ = 1
## All Components
**Non-zero** (even permutations of 123):
- ε₁₂₃ = ε₂₃₁ = ε₃₁₂ = +1
**Non-zero** (odd permutations of 123):
- ε₁₃₂ = ε₃₂₁ = ε₂₁₃ = -1
**Zero** (any repeated index):
- ε₁₁₂ = ε₁₂₂ = ε₁₁₁ = ... = 0
## Angular Momentum Commutators
The commutation relations $[\hat L_i, \hat L_j] = iℏ \sum_k ε_{ijk} \hat L_k$ are expressed compactly as:
$$[\hat L_i, \hat L_j] = iℏ \sum_{k=1}^3 ε_{ijk} \hat L_k$$where i, j, k ∈ {1, 2, 3} represent {x, y, z}.
## Cross Product Expression
$$\hat L_i = \sum_{j=1}^3 \sum_{k=1}^3 ε_{ijk} \hat x_j \hat P_k$$

This is equivalent to $\hat L = \hat r \times \hat P$.
**Example** (z-component):
$$\hat L_z = \hat L_3 = \sum_j \sum_k ε_{3jk} \hat x_j \hat P_k  = ε_{312}\hat x_1\hat P_2 + ε_{321}\hat x_2\hat P_1  = \hat x \hat P_y - \hat y\hat P_x$$
Related: [[Orbital Angular Momentum as Generator of Rotations]], [[Commutation Relations]]
