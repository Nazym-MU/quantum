Differential operators representing orbital angular momentum in spherical coordinates.
Position states in spherical coordinates: $|r, \theta, \phi\rangle$
The angles $\theta$ (polar) and $\phi$ (azimuthal) specify direction, while $r$ specifies magnitude.
## $L_z$ Component
$$\hat{L}_z \rightarrow -i\hbar \frac{\partial}{\partial \phi}$$
**Derivation**: From $\hat{R}(d\phi \hat{k})|r, \theta, \phi\rangle = |r, \theta, \phi + d\phi\rangle$ and the generator form $\hat{R}(d\phi \hat{k}) = 1 - (i/\hbar)\hat{L}_z d\phi$.
This is analogous to linear momentum: $\hat{p}_x \rightarrow \frac{\hbar}{i} \frac{\partial}{\partial x}$
[[Deriving L_z in Position Space]]
## $L_x$ and $L_y$ Components
$$\hat{L}_x \rightarrow -i\hbar\left(\sin\phi \frac{\partial}{\partial \theta} + \cot\theta \cos\phi \frac{\partial}{\partial \phi}\right)$$
$$\hat{L}_y \rightarrow -i\hbar\left(-\cos\phi \frac{\partial}{\partial \theta} + \cot\theta \sin\phi \frac{\partial}{\partial \phi}\right)$$
These are derived by expressing $\hat{L} = \hat{r} \times \hat{p}$ in spherical coordinates. We know:
$$\hat L \to ru_r \times(-i\hbar)\left( u_r \frac{\partial}{\partial r} + u_\theta \frac{1}{r} \frac{\partial}{\partial \theta} + u_\phi \frac{1}{r\sin\theta}\frac{\partial}{\partial \phi} \right) = -i\hbar\left(  u_\phi \frac{\partial}{\partial \theta} + u_\theta \frac{1}{\sin\theta}\frac{\partial}{\partial \phi} \right) $$
## L² Operator

$$\hat{L}^2 \rightarrow -\hbar^2 \left[\frac{1}{\sin\theta}\frac{\partial}{\partial \theta}\left(\sin\theta \frac{\partial}{\partial \theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2}{\partial \phi^2}\right]$$
This is the angular part of the Laplacian in spherical coordinates.
## Key Property
All angular momentum operators depend only on angles $(\theta, \phi)$, not on radius $r$. This reflects that rotations change direction but not magnitude.
## Physical Significance
These differential operators allow us to solve eigenvalue equations:
$$\hat{L}_z \langle \theta, \phi | l, m \rangle = m\hbar \langle \theta, \phi | l, m \rangle$$
becomes a differential equation for the spherical harmonics.
Related: [[Single-Valuedness and Integer Angular Momentum]], [[Laplacian in Spherical Coordinates]]
