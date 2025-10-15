Derivation: ⟨+b|+a⟩ = cos(θ_ab/2)
## Starting Point
For spin-1/2 particle, eigenstate of spin along axis **a** (at angle θ_a from z) and  **b** (at angle θ_b):
$$|+a\rangle = \cos\frac{\theta_a}{2}|+z\rangle + \sin\frac{\theta_a}{2}|-z\rangle \qquad |+b\rangle = \cos\frac{\theta_b}{2}|+z\rangle + \sin\frac{\theta_b}{2}|-z\rangle$$

These are eigenstates of $\hat{S} \cdot \hat{a}$ and $\hat{S} \cdot \hat{b}$ with eigenvalue +ℏ/2.
## Inner Product
$$\langle +b|+a\rangle = \left(\cos\frac{\theta_b}{2}\langle +z| + \sin\frac{\theta_b}{2}\langle -z|\right)\left(\cos\frac{\theta_a}{2}|+z\rangle + \sin\frac{\theta_a}{2}|-z\rangle\right) = \cos\frac{\theta_b}{2}\cos\frac{\theta_a}{2} + \sin\frac{\theta_b}{2}\sin\frac{\theta_a}{2}$$
Cosine Addition:
$$\cos(A - B) = \cos A \cos B + \sin A \sin B$$
$$\langle +b|+a\rangle = \cos\left(\frac{\theta_b - \theta_a}{2}\right)$$
Angle between the two axes:
$$\theta_{ab} = \theta_b - \theta_a$$
Therefore:
$$\boxed{\langle +b|+a\rangle = \cos\frac{\theta_{ab}}{2}}$$
- θ_ab = 0 (same axis): cos(0) = 1 → states identical 
- θ_ab = 90°: cos(45°) = 1/√2 (50% overlap)
- θ_ab = 180° (opposite): cos(90°) = 0 → orthogonal 