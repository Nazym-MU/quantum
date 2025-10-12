### Method 1: Direct Superposition
**Single-particle**:
$$|+x\rangle = \frac{1}{\sqrt{2}}|+z\rangle + \frac{1}{\sqrt{2}}|-z\rangle$$
**Apply to particle 1** in |+x,+z⟩:
$$|+x,+z\rangle = |+x\rangle_1|+z\rangle_2 = \left(\frac{1}{\sqrt{2}}|+z\rangle_1 + \frac{1}{\sqrt{2}}|-z\rangle_1\right)|+z\rangle_2$$
$$= \frac{1}{\sqrt{2}}|+z\rangle_1|+z\rangle_2 + \frac{1}{\sqrt{2}}|-z\rangle_1|+z\rangle_2 = \frac{1}{\sqrt{2}}|+z,+z\rangle + \frac{1}{\sqrt{2}}|-z,+z\rangle$$
### Method 2: Rotation Operators
Use $\hat{R}_1 \otimes \hat{I}_2$ to rotate only particle 1.
**Single-particle rotation**:
$$|+x\rangle = \hat{R}\left(\frac{\pi}{2}\hat{j}\right)|+z\rangle$$
**Apply to two-particle state**:
$$|+x,+z\rangle = \left[\hat{R}_1\left(\frac{\pi}{2}\hat{j}\right) \otimes \hat{I}_2\right]|+z,+z\rangle= \hat{R}_1\left(\frac{\pi}{2}\hat{j}\right)|+z\rangle_1 \otimes |+z\rangle_2 = |+x\rangle_1 \otimes |+z\rangle_2$$
## Example: Both Particles in x-Basis
**Goal**: Express |+x,+x⟩ in S_z basis.

$$|+x,+x\rangle = |+x\rangle_1|+x\rangle_2= \left(\frac{1}{\sqrt{2}}|+z\rangle_1 + \frac{1}{\sqrt{2}}|-z\rangle_1\right)\left(\frac{1}{\sqrt{2}}|+z\rangle_2 + \frac{1}{\sqrt{2}}|-z\rangle_2\right)$$
$$= \frac{1}{2}|+z,+z\rangle + \frac{1}{2}|+z,-z\rangle + \frac{1}{2}|-z,+z\rangle + \frac{1}{2}|-z,-z\rangle$$
Equal superposition of all four basis states.
## Matrix Form
In the 4D product basis {|+z,+z⟩, |+z,-z⟩, |-z,+z⟩, |-z,-z⟩}:
**Transformation matrix** for particle 1:
$$S_1 = S \otimes I = \begin{pmatrix} S_{11} & S_{12} & 0 & 0 \\ S_{21} & S_{22} & 0 & 0 \\ 0 & 0 & S_{11} & S_{12} \\ 0 & 0 & S_{21} & S_{22} \end{pmatrix}$$
## Related
- [[Direct Product of Vector Spaces]]