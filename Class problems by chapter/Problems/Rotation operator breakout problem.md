1. How would you calculate the action of $\hat{R}(\phi j) = e^{-iJ_y/\hbar}$ acting on a state $\ket{+z}$? What is it physically? What is it mathematically?
2. Is |+z> an eigenstate of $\hat R(j)$?  When $\phi=\pi/2$ , what is the result of the action of $\hat R(j)$ on $\ket{+z}$? Did you expect this?
---
## Solution
This one is about being able to expand Taylor series.
One way is to use spin operators, and another way is using ladder operators. Using $\sigma_y=\begin{pmatrix}0 & -i \\ i & 0 \end{pmatrix}$:
$$J_y = \frac{\hbar}{2}\sigma_y$$
Knowing the property $\sigma_y = I$ and expanding the Taylor series:

$$\hat{R}(\phi) = e^{-i\sigma_y\phi/2} = I + (-i\sigma_y\phi/2) + \frac{(-i\sigma_y\phi/2)^2}{2!} + \frac{(-i\sigma_y\phi/2)^3}{3!} + \cdots$$
Powers of $\sigma_y$:
$$\sigma_y = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}$$
$$\sigma_y^2 = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}\begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$$
$$\sigma_y^3 = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix} = \sigma_y$$
Separate:
$$e^{-i\sigma_y\phi/2} = \left(1 - \frac{(\phi/2)^2}{2!} + \cdots\right)I + \left(\frac{-i\phi}{2} + \frac{i(\phi/2)^3}{3!} - \cdots\right)\sigma_y$$
$$= \cos\frac{\phi}{2}I - i\sin\frac{\phi}{2}\sigma_y = \begin{bmatrix} \cos\frac{\phi}{2} & 0 \\ 0 & \cos\frac{\phi}{2} \end{bmatrix} - i\sin\frac{\phi}{2}\begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix} = \begin{bmatrix} \cos\frac{\varphi}{2} & -\sin\frac{\varphi}{2} \\ \sin\frac{\varphi}{2} & \cos\frac{\varphi}{2} \end{bmatrix}$$
## Operator acting on $\ket{+z}$:
$$\ket{+z} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}$$ in the $S_z$ basis
$$\hat{R}(\phi)\ket{+z} = \begin{bmatrix} \cos\frac{\phi}{2} & -\sin\frac{\phi}{2} \\ \sin\frac{\phi}{2} & \cos\frac{\phi}{2} \end{bmatrix}\begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} \cos(\phi/2) \\ \sin(\phi/2) \end{bmatrix}$$
Result: $$\hat{R}(\phi)\ket{+z} = \cos\frac{\phi}{2}|+z\rangle + \sin\frac{\phi}{2}|-z\rangle$$
**Not an eigenstate** (actually eigenstates of $\hat{J}_y$)
## When $\phi = \frac{\pi}{2}$:
$$\hat{R}(\phi)\ket{+z} = \cos\frac{\pi}{4}|+z\rangle + \sin\frac{\pi}{4}|-z\rangle = \frac{1}{\sqrt{2}}|+z\rangle + \frac{1}{\sqrt{2}}|-z\rangle = |+x\rangle$$
