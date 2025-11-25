To convert between bases, use completeness:
$$|+x\rangle = (|+z\rangle\langle+z| + |-z\rangle\langle-z|)|+x\rangle = |+z\rangle\langle+z|+x\rangle + |-z\rangle\langle-z|+x\rangle$$
## Active and Passive Transformations
- Active Transformation: **Rotate the state**, keep the basis fixed: $|\psi'\rangle = \hat{R}|\psi\rangle$
	- Physical state changes
	- Basis vectors stay the same
- Passive Transformation: **Rotate the basis**, keep the state fixed
	- Operation $R^\dagger$, but changing coordinate system
	- Physical state unchanged
#### [[Example - Rotating by 90° about y-axis]]
$$|\psi'\rangle \xrightarrow[S_z]{} \begin{pmatrix} \langle+z|\psi'\rangle \\ \langle-z|\psi'\rangle \end{pmatrix} = \begin{pmatrix} \langle+z|\hat{R}^\dagger|\psi\rangle \\ \langle-z|\hat{R}^\dagger|\psi\rangle \end{pmatrix} = \begin{pmatrix} \langle+x|\psi\rangle \\ \langle-x|\psi\rangle \end{pmatrix} \xleftarrow[S_x]{} |\psi\rangle$$

Left to right - active, right to left - passive
Transformation of operators - [[S-Matrix and Basis Changes]]
## Related
- [[Basis States and Completeness]]