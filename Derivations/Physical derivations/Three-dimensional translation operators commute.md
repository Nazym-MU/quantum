$$\hat T(a_x\hat i), \hat T(a_y\hat j)] = 0$$
More generally, translations in any two different directions commute.
## Proof using series expansion
Starting from $\,\hat T(a) = e^{-i\hat P\cdot a/\hbar}\,$, expand to second order:
$$
\hat T(a_x \hat{\mathbf{i}}) =
1 - \frac{i}{\hbar}\hat p_x a_x
- \frac{1}{2}\left(\frac{\hat p_x a_x}{\hbar}\right)^2 + \cdots
$$
$$
\hat T(a_y \hat{\mathbf{j}}) =
1 - \frac{i}{\hbar}\hat p_y a_y
- \frac{1}{2}\left(\frac{\hat p_y a_y}{\hbar}\right)^2 + \cdots
$$
## Product
$$
\hat T(a_x \hat{\mathbf{i}})\,\hat T(a_y \hat{\mathbf{j}})
=
\left[1 - \frac{i}{\hbar}\hat p_x a_x - \frac{1}{2}\left(\frac{\hat p_x a_x}{\hbar}\right)^2 + \cdots\right]
\left[1 - \frac{i}{\hbar}\hat p_y a_y - \frac{1}{2}\left(\frac{\hat p_y a_y}{\hbar}\right)^2 + \cdots\right]
$$
Expanding through second order and using $[\hat p_x, \hat p_y] = 0$:
$$
=
1
- \frac{i}{\hbar}(\hat p_x a_x + \hat p_y a_y)
- \frac{1}{2\hbar^2}
\left(
\hat p_x^2 a_x^2
+ \hat p_y^2 a_y^2
+ 2\hat p_x \hat p_y a_x a_y
\right)
+ \cdots
$$
Reversing Order $\hat T(a_y \hat{\mathbf{j}})\,\hat T(a_x \hat{\mathbf{i}})$ gives the identical expression because the momentum operators commute.
Since the products commute for arbitrary $a_x, a_y$, the generators must commute. This extends to all components:
$$
[\hat p_i, \hat p_j] = 0.
$$

Related: [[Three-Dimensional Translation Operator]], [[Position-Momentum Commutation Relations in 3D]]
