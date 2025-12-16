Operator that shifts position of a particle in 3D space.
## Definition
T̂(a)|r⟩ = |r + a⟩
For component-wise translations:
- T̂(aₓî)|x, y, z⟩ = |x + aₓ, y, z⟩
- T̂(aᵧĵ)|x, y, z⟩ = |x, y + aᵧ, z⟩
- T̂(aᵧk̂)|x, y, z⟩ = |x, y, z + aᵧ⟩
$$\hat T(a) = e^{-i\hat P\cdot a/ℏ}$$
The momentum operator $\hat P$ is the generator of spatial translations.

## Key Property: Translations Commute
Unlike rotations, translations in different directions commute:
$$[\hat T(a_x\hat i), \hat T(a_y\hat j)] = 0$$

**Mathematical consequence**: $[\hat P_i, \hat P_j] = 0$ for all i, j
Simultaneous momentum eigenstates in all three directions.
Related: [[Position-Momentum Commutation Relations in 3D]], [[Three-dimensional translation operators commute]], [[Rotation Operators]]
