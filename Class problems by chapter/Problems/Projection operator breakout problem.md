1. Why do we need to normalize |w> in order to construct a projection operator out of it? 
2. Construct the projection operator that projects a vector |v> onto |w>
3. Show that $\hat P = \hat P^2$.
4. Construct the orthogonal projection operator, $P_\perp$.
5. Verify that your operators satisfy the properties of a generic projection operator.
---
## Solution
### 1. Why normalize: because $\hat{P}^2 = \hat{P}$ must hold true.
$\hat{P} = |w\rangle\langle w|$ unnormalized will produce:
$$\hat{P}^2 = |w\rangle\langle w|w\rangle\langle w| = \langle w|w\rangle|w\rangle\langle w| = \langle w|w\rangle\hat{P}$$
must be normalized
### 2. Construct a projection operator that projects $|v\rangle$ onto $|w\rangle$:
Normalize: 
$$\hat{P} = \frac{|w\rangle\langle w|}{\langle w|w\rangle}$$
Projection: 
$$\hat{P}|v\rangle = \frac{|w\rangle\langle w|}{\langle w|w\rangle}|v\rangle = \frac{\langle w|v\rangle|w\rangle}{\langle w|w\rangle}$$
### 3. Prove that $\hat{P}^2 = \hat{P}$:
$$\hat{P}^2|v\rangle = \frac{|w\rangle\langle w||w\rangle\langle w|}{\langle w|w\rangle^2}|v\rangle = \frac{|w\rangle\langle w|}{\langle w|w\rangle}|v\rangle$$
### 4. Orthogonal projection $P_\perp$:
$$\hat{P}_\perp = \hat{I} - \hat{P} = \hat{I} - \frac{|w\rangle\langle w|}{\langle w|w\rangle}$$

$$\hat{P}_\perp|v\rangle = |v\rangle - \frac{|w\rangle\langle w|v\rangle}{\langle w|w\rangle}$$
### 5. Verify properties:
#### (1) $P_\perp^2 = P_\perp$

$$\left(\hat{I} - \frac{|w\rangle\langle w|}{\langle w|w\rangle}\right)^2 = \hat{I} - 2\frac{|w\rangle\langle w|}{\langle w|w\rangle} + \frac{|w\rangle\langle w||w\rangle\langle w|}{\langle w|w\rangle^2} = \hat{I} - \frac{|w\rangle\langle w|}{\langle w|w\rangle}$$
#### (2) Hermiticity: $\hat{P}_\perp^\dagger = \hat{P}_\perp$
$$\hat{P}^\dagger = \frac{(|w\rangle\langle w|)^\dagger}{\langle w|w\rangle^*} = \frac{|w\rangle\langle w|}{\langle w|w\rangle} = \hat{P}$$
$$\hat{P}_\perp^\dagger = (\hat{I} - \hat{P})^\dagger = \hat{I}^\dagger - \hat{P}^\dagger = \hat{I} - \hat{P}$$
#### (3) Orthogonality: $\hat{P}\hat{P}_\perp = 0$

$$\hat{P}(\hat{I} - \hat{P}) = \hat{P}\hat{I} - \hat{P}^2 = \hat{P} - \hat{P} = 0$$
#### (4) Completeness: $\hat{P} + \hat{P}_\perp = \hat{I}$
$$\hat{P} + \hat{I} - \hat{P} = \hat{I}$$