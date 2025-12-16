Derivation showing how kinetic energy separates into radial and rotational parts.
## Starting Identity
$$(\hat{\mathbf r} \cdot \hat{\mathbf p})^{2} = \hat p^{\,2} - \dfrac{\hat L^{\,2}}{r^{2}}$$

## Proof of Identity
Start with:
$$ \hat L^{\,2} = (\hat{\mathbf r} \times \hat{\mathbf p}) \cdot (\hat{\mathbf r} \times \hat{\mathbf p})$$

Using the vector identity  $(\mathbf A \times \mathbf B)\cdot(\mathbf A \times \mathbf B) = A^{2}B^{2} - (\mathbf A\cdot\mathbf B)^{2}$:
$$ \hat L^{\,2} = r^{2}\hat p^{\,2} - (\hat{\mathbf r}\cdot \hat{\mathbf p})^{2} $$
Rearranging:
$$ (\hat{\mathbf r}\cdot \hat{\mathbf p})^{2} = r^{2}\hat p^{\,2} - \hat L^{\,2} $$
Dividing by $r^{2}$:
$$ \dfrac{(\hat{\mathbf r}\cdot \hat{\mathbf p})^{2}}{r^{2}}
= \hat p^{\,2} - \dfrac{\hat L^{\,2}}{r^{2}} $$

## Position Space Evaluation
In position space:
$$ \bra{r} (\hat{\mathbf r}\cdot\hat{\mathbf p}) \ket{\psi}
= \bra{r}\hat{\mathbf r}\ket{\psi} \cdot \bra{r}\hat{\mathbf p}\ket{\psi} $$
Since $\bra{r}\hat{\mathbf r}\ket{\psi} = r\,\bra{r}\psi\rangle$  
and $\bra{r}\hat{\mathbf p}\ket{\psi} = -i\hbar\nabla\bra{r}\psi\rangle$:
$$
\bra{r}(\hat{\mathbf r}\cdot\hat{\mathbf p})\ket{\psi}
= r \cdot (-i\hbar\nabla\bra{r}\psi\rangle)
= -i\hbar\, r\, \frac{\partial}{\partial r}\bra{r}\psi\rangle
$$
In spherical coordinates, the dot product selects the radial derivative:
$$ \hat{\mathbf r}\cdot\nabla = \frac{\partial}{\partial r} $$
so:
$$ \bra{r}(\hat{\mathbf r}\cdot\hat{\mathbf p})\ket{\psi}
= -i\hbar\, r\, \frac{\partial}{\partial r}\bra{r}\psi\rangle $$
## Second Power
$$ \bra{r}(\hat{\mathbf r}\cdot\hat{\mathbf p})^{2}\ket{\psi}
= -\hbar^{2} r \frac{\partial}{\partial r}
\left( r\frac{\partial}{\partial r}\bra{r}\psi\rangle \right) $$
$$
= -\hbar^{2} r\left( \frac{\partial^{2}}{\partial r^{2}}
+ \frac{1}{r}\frac{\partial}{\partial r} \right)
r\,\bra{r}\psi\rangle
$$
$$
= -\hbar^{2}\left( r^{2}\frac{\partial^{2}}{\partial r^{2}}
+ r\frac{\partial}{\partial r} \right)\bra{r}\psi\rangle
$$
## Kinetic Energy Decomposition
$$
\bra{r}\frac{\hat p^{\,2}}{2\mu}\ket{\psi}
= \bra{r}\left( \frac{(\hat{\mathbf r}\cdot\hat{\mathbf p})^{2}}{2\mu r^{2}}
+ \frac{\hat L^{\,2}}{2\mu r^{2}} \right)\ket{\psi}
$$
Radial part:
$$
-\frac{\hbar^{2}}{2\mu}
\left( \frac{\partial^{2}}{\partial r^{2}}
+ \frac{2}{r}\frac{\partial}{\partial r} \right)
\bra{r}\psi\rangle
$$

Rotational part:
$$ \bra{r}\frac{\hat L^{\,2}}{2\mu r^{2}}\ket{\psi} $$
**Physical interpretation**:
- First term: **radial kinetic energy**
- Second term: **rotational kinetic energy**  
  $$ \hat L^{\,2}/2I \text{ with } I = \mu r^{2} $$

Related: [[Radial Schrödinger Equation]], [[Radial Momentum Operator]], [[Effective Potential in Central Force Problem]]
