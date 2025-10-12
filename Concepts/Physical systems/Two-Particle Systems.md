For two spin-1/2 particles, the state space is:
$$\mathcal{H} = \mathcal{H}_1 \otimes \mathcal{H}_2$$
**Dimension**: 2 × 2 = 4 (four independent states)
### Single-Particle Operators
Act only on one particle:
$$\hat{S}_{1z} \otimes \hat{I}_2 \quad \text{(acts on particle 1 only)}$$
Example:
$$(\hat{S}_{1z} \otimes \hat{I}_2)|+z,-z\rangle = \left(\frac{\hbar}{2}\right)|+z,-z\rangle$$
### Two-Particle Operators
$$\hat{S}_1 \cdot \hat{S}_2 = \hat{S}_{1x}\hat{S}_{2x} + \hat{S}_{1y}\hat{S}_{2y} + \hat{S}_{1z}\hat{S}_{2z}$$
-  [[Spin-Spin Interaction]]
## Commutation Relations
- Individual particles commute: $[\hat{S}_{1i}, \hat{S}_{2j}] = 0 \quad \forall i,j$
	- Can rotate each particle independently.
- Components of same particle don't commute: $[\hat{S}_{1x}, \hat{S}_{1y}] = i\hbar\hat{S}_{1z}$
> [[Basis Transformations Two-Particle]] 
## Total Angular Momentum Basis
Alternative basis using [[Total Angular Momentum]]:
- **Singlet**: $|s=0, m=0\rangle = \frac{1}{\sqrt{2}}(|+z,-z\rangle - |-z,+z\rangle)$
- **Triplet**: $|s=1, m\rangle$ (3 states)
These are eigenstates of $\hat{S}^2_{\text{total}}$ and $\hat{S}_{\text{total},z}$.
## Physical Examples
- **[[Hyperfine Splitting]]**: Electron-proton spin interaction in hydrogen\
## Related
- [[Direct Product of Vector Spaces]]
- [[Total Angular Momentum]]
- [[Spin-Spin Interaction]]
- [[Hyperfine Splitting]]
- [[(16)]] for basis transformation details