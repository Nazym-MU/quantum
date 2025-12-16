## Position Eigenstates
**Definition**: |r⟩ = |x, y, z⟩ where
- x̂|r⟩ = x|r⟩
- ŷ|r⟩ = y|r⟩  
- ẑ|r⟩ = z|r⟩
**Orthogonality**: $$⟨r|r'⟩ = δ³(r - r') = δ(x - x')δ(y - y')δ(z - z')$$The 3D Dirac delta function is the product of three 1D delta functions.
## Momentum Eigenstates
**Definition**: |p⟩ with simultaneous eigenvalues $p_x, p_y, p_z$
- $\hat p_x|p⟩ = p_x|p⟩$
- $\hat p_y|p⟩ = p_y|p⟩$
- $\hat p_z|p⟩ = p_z|p⟩$
**Orthogonality**: $⟨p|p'⟩ = δ^3(p - p')$
**Position representation**: $⟨r|p⟩ = \frac{1}{(2πℏ)^{3/2}}e^{ip\cdot r/ℏ}$
This is the product of three 1D plane waves.
## Generic State Expansion
Any state $|ψ⟩$ can be expanded in either basis:
**Position basis**: $\ket\psi = \int d^3r \ket{r}\bra r ψ⟩$
**Momentum basis**: $\ket\psi = \int d^3p \ket{p}\bra p ψ⟩$
## Probability Interpretation
**Position space**: d³r|⟨r|ψ⟩|² = probability of finding particle in volume d³r at position r
**Momentum space**: d³p|⟨p|ψ⟩|² = probability of finding momentum between p and p + dp
## Normalization
$⟨ψ|ψ⟩ = \int d^3r|⟨r|ψ⟩|² = \int d^3p|⟨p|ψ⟩|^2 = 1$
Related: [[Position-Momentum Commutation Relations in 3D]], [[Wave Function]]
