At each matrix entry, we have $\braket{j, m'|\hat J_x|j, m}$

$$\hat{J}_+ = \hat{J}_x + i\hat{J}_y \qquad \hat{J}_- = \hat{J}_x - i\hat{J}_y$$
$$\Rightarrow \hat{J}_x = \frac{\hat{J}_+ + \hat{J}_-}{2} \qquad \hat{J}_y = \frac{\hat{J}_+ - \hat{J}_-}{2i}$$
### Start with $\hat{J}_z$ (easiest):
$$\hat{J}_z|j,m\rangle = m\hbar|j,m\rangle$$
Matrix elements: $\langle 1,m_i|\hat{J}_z|1,m_j\rangle$
$$\hat{J}_z|1,1\rangle = \hbar|1,1\rangle \qquad \hat{J}_z|1,0\rangle = 0|1,0\rangle \qquad \hat{J}_z|1,-1\rangle = -\hbar|1,-1\rangle$$
$$\boxed{\hat{J}_z = \hbar\begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & -1 \end{bmatrix}}$$
### Ladder operators:
$$\hat{J}_+|j,m\rangle = \sqrt{j(j+1) - m(m+1)}\hbar|j,m+1\rangle$$
$$\hat{J}_-|j,m\rangle = \sqrt{j(j+1) - m(m-1)}\hbar|j,m-1\rangle$$
### For $j=1$:
$$\hat{J}_+|1,1\rangle = 0 \qquad \hat{J}_+|1,0\rangle = \sqrt{2}\hbar|1,1\rangle \qquad \hat{J}_+|1,-1\rangle = \sqrt{2}\hbar|1,0\rangle$$
$$\hat{J}_-|1,1\rangle = \sqrt{2}\hbar|1,0\rangle \qquad \hat{J}_-|1,0\rangle = \sqrt{2}\hbar|1,-1\rangle \qquad \hat{J}_-|1,-1\rangle = 0$$
$$\hat{J}_+ = \hbar\begin{bmatrix} 0 & \sqrt{2} & 0 \\ 0 & 0 & \sqrt{2} \\ 0 & 0 & 0 \end{bmatrix} \qquad \hat{J}_- = \hbar\begin{bmatrix} 0 & 0 & 0 \\ \sqrt{2} & 0 & 0 \\ 0 & \sqrt{2} & 0 \end{bmatrix}$$
$$\boxed{\hat{J}_x = \frac{\hbar}{\sqrt{2}}\begin{bmatrix} 0 & 1 & 0 \\ 1 & 0 & 1 \\ 0 & 1 & 0 \end{bmatrix}} \qquad \boxed{\hat{J}_y = \frac{\hbar}{\sqrt{2}}\begin{bmatrix} 0 & -i & 0 \\ i & 0 & -i \\ 0 & i & 0 \end{bmatrix}}$$