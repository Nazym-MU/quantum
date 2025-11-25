What is the matrix representation of $\hat J_z$ using the states $|+y\rangle$ and $|-y\rangle$  as a basis? Use this representation to evaluate the expectation value of $S_z$ for a collection of particles each in the state $|-y\rangle$ .

---
## Solution
$$\hat{J}_z \xrightarrow[S_z \text{ basis}]{} \frac{\hbar}{2}\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$$
$$|+y\rangle = \frac{1}{\sqrt{2}}|+z\rangle + \frac{i}{\sqrt{2}}|-z\rangle \qquad |-y\rangle = \frac{1}{\sqrt{2}}|+z\rangle - \frac{i}{\sqrt{2}}|-z\rangle$$
$S_y \rightarrow S_z$ basis: 
$$\begin{bmatrix} \langle +z|+y\rangle & \langle +z|-y\rangle \\ \langle -z|+y\rangle & \langle -z|-y\rangle \end{bmatrix} = \frac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ i & -i \end{bmatrix}$$
Using the change-of-basis + transformation formula ($P^{-1}AP$, where $P^{-1}$ is the conjugate transpose):
$$\hat{J}_z \xrightarrow{S_y \text{ basis}} \frac{\hbar}{4}\begin{bmatrix} 1 & -i \\ 1 & i \end{bmatrix}\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}\begin{bmatrix} 1 & 1 \\ i & -i \end{bmatrix} = \frac{\hbar}{4}\begin{bmatrix} 1 & -i \\ 1 & i \end{bmatrix}\begin{bmatrix} 1 & 1 \\ -i & i \end{bmatrix}$$
$$= \frac{\hbar}{4}\begin{bmatrix} 0 & 2 \\ 2 & 0 \end{bmatrix} = \frac{\hbar}{2}\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} = \frac{\hbar}{2}\sigma_x$$
### Expectation: $|-y\rangle \rightarrow \begin{bmatrix} 0 \\ 1 \end{bmatrix}$ in $S_y$ basis
$$\langle \hat{J}_z \rangle = \langle -y|\hat{J}_z|-y\rangle = \frac{\hbar}{2}\begin{bmatrix} 0 & 1 \end{bmatrix}\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}\begin{bmatrix} 0 \\ 1 \end{bmatrix} = \frac{\hbar}{2}\begin{bmatrix} 0 & 1 \end{bmatrix}\begin{bmatrix} 1 \\ 0 \end{bmatrix}$$
$$= \frac{\hbar}{2} \cdot 0 = 0$$