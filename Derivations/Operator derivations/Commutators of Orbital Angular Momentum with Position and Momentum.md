Derivation of how $\hat L_z$ commutes with $\hat p^{\,2}$ and $r^{2}$ (and thus with kinetic and potential energy).
## Commutators with Momentum Components
Starting from $\hat L_z = x \hat p_y - y \hat p_x$:
**$[\hat L_z, \hat p_x]$**:
$$[\hat L_z, \hat p_x]
= [x \hat p_y - y \hat p_x, \hat p_x]
= [x\hat p_y, \hat p_x] \quad \text{(second term commutes)}
= [x, \hat p_x]\hat p_y
= i\hbar\,\hat p_y$$
**$[\hat L_z, \hat p_y]$**:
$$[\hat L_z, \hat p_y]
= [x\hat p_y - y\hat p_x, \hat p_y]
= -[y\hat p_x, \hat p_y]
= -[y, \hat p_y]\hat p_x
= -i\hbar\,\hat p_x$$
**$[\hat L_z, \hat p_z] = 0$**
because $\hat L_z$ does not involve $z$ or $\hat p_z$.
## Commutator with $\hat p^{\,2}$
$[\hat L_z, \hat p^{\,2}] = [\hat L_z, \hat p_x^{\,2} + \hat p_y^{\,2} + \hat p_z^{\,2}]$
For the $\hat p_x^{\,2}$ term:
$$[\hat L_z, \hat p_x^{\,2}]
= [\hat L_z, \hat p_x]\hat p_x + \hat p_x[\hat L_z, \hat p_x]
= i\hbar\,\hat p_y\hat p_x + i\hbar\,\hat p_x\hat p_y
= 2i\hbar\,\hat p_x\hat p_y$$
Similarly for $\hat p_y^{\,2}$:
$$[\hat L_z, \hat p_y^{\,2}]
= -2i\hbar\,\hat p_x\hat p_y$$
For $\hat p_z^{\,2}$:
$$[\hat L_z, \hat p_z^{\,2}] = 0$$
**Total:**
$$[\hat L_z, \hat p^{\,2}]
= 2i\hbar\,\hat p_x\hat p_y - 2i\hbar\,\hat p_x\hat p_y = 0$$
## Commutators with Position Components
By a similar calculation:
$$[\hat L_z, x] = i\hbar\,y$$
$$[\hat L_z, y] = -i\hbar\,x$$
$$[\hat L_z, z] = 0$$
## Commutator with $r^{2}$
$$[\hat L_z, r^{2}]
= [\hat L_z, x^{2} + y^{2} + z^{2}]
= [\hat L_z, x^{2}] + [\hat L_z, y^{2}]
= 2i\hbar\,xy - 2i\hbar\,xy
= 0$$
## Physical Consequence
Since $[\hat L_z, \hat p^{\,2}] = 0$ and $[\hat L_z, r^{2}] = 0$:
- $[\hat L_z, \hat p^{\,2}/2\mu] = 0$ → kinetic energy is invariant  
- $[\hat L_z, V(r)] = 0$ → potential energy is invariant (since $V$ depends only on $r = |\mathbf r|$)  
- Therefore:  
$$[\hat L_z, \hat H] = 0$$
showing rotational invariance.
The same arguments apply to $\hat L_x$ and $\hat L_y$ by symmetry.
Related: [[Orbital Angular Momentum as Generator of Rotations]], [[Rotational Invariance and Angular Momentum Conservation]]
