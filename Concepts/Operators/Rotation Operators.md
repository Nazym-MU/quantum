$\hat{R}(\theta\hat{n})$ rotates by angle θ about axis $\hat{n}$.
## Finite Rotation
For rotation by angle φ about z-axis:
$$\hat{R}(\phi\hat{k}) = e^{-i\hat{J}_z\phi/\hbar}$$
The generator Ĵ_z determines how rotation acts.
## Infinitesimal Rotation
For small dφ, [[Taylor Expansion for Rotation Operator|Taylor expand]]:
$$\hat{R}(d\phi\hat{k}) = 1 - \frac{i}{\hbar}\hat{J}_z d\phi + O(d\phi^2) \approx 1 - \frac{i}{\hbar}\hat{J}_z d\phi$$
## Properties
- Unitary: $\hat{R}^\dagger\hat{R} = \hat{I}$, preserves normalization (probability conservation).
- Composition: $\hat{R}(\phi_2\hat{k})\hat{R}(\phi_1\hat{k}) = \hat{R}((\phi_1+\phi_2)\hat{k})$. Rotations about same axis add.
- Inverse: $\hat{R}^{-1}(\phi\hat{k}) = \hat{R}(-\phi\hat{k}) = \hat{R}^\dagger(\phi\hat{k})$
## Action on Eigenstates
Rotating eigenstate about its own axis: $\hat{R}(\phi\hat{k})|+z\rangle = e^{-i\phi/2}|+z\rangle$, only picks up phase factor $e^{-i\phi/2}$ (eigenvalue −ℏ/2).
### Adjoint rotation
- Rotates in opposite direction (inverse operation).
- Acts on bras: $\langle+z|\hat{R}^\dagger$
## Matrix Representation
In S_z basis for 90° rotation about y:
$$\hat{R}\left(\frac{\pi}{2}\hat{j}\right) \rightarrow \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & -1 \\ 1 & 1 \end{pmatrix}$$
## Related
- [[Rotation Operator from Infinitesimal]]
- [[Angular Momentum Operators]]
- [[Unitary Operators]]
- [[Basis Transformations]]