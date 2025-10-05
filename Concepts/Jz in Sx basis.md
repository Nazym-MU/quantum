$\ket{+x} = \frac{1}{\sqrt{2}}\ket{+z} + \frac{1}{\sqrt{2}}\ket{-z}$
$\ket{-x} = \frac{1}{\sqrt{2}}\ket{+z} - \frac{1}{\sqrt{2}}\ket{-z}$ 
$$\mathbb{S} = \begin{pmatrix} \langle +z | +x \rangle & \langle +z | -x \rangle \\ \langle -z | +x \rangle & \langle -z | -x \rangle \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$$
$$\hat{J}_z \xrightarrow[S_x\,\text{basis}]{} \begin{pmatrix} \braket{+x|+z} & \braket{+x|-z} \\ \braket{-x|+z} & \braket{-x|-z} \end{pmatrix} \begin{pmatrix} \braket{+z|\hat{J}_z|+z} & \braket{+z|\hat{J}_z|-z} \\ \braket{-z|\hat{J}_z|+z} & \braket{-z|\hat{J}_z|-z} \end{pmatrix}\begin{pmatrix} \braket{+z|+x} & \braket{+z|-x} \\ \braket{-z|+x} & \braket{-z|-x} \end{pmatrix} =$$
$$=\frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \frac{\hbar}{2} \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} = \frac{\hbar}{2} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$$
Matrix representation of $J_z$ in $S_x$ basis is no longer diagonal because we're not using the eigenstates as the basis.

Eigenstate $\ket{+z}$ in the $S_x$ basis:
$$\ket{+z} \xrightarrow[S_x\,\text{basis}]{} \frac{1}{\sqrt2}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\begin{pmatrix} 1  \\ 0 \end{pmatrix} = \frac{1}{\sqrt2}\begin{pmatrix} 1 \\ 1 \end{pmatrix}$$
Eigenvalue equation in the $S_x$ basis:
$$\hat{J}_z\ket{+z} \xrightarrow[S_x\,\text{basis}]{} \frac{\hbar}{2}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\frac{1}{\sqrt2}\begin{pmatrix} 1  \\ 0 \end{pmatrix} = \frac{\hbar}{2\sqrt 2} \begin{pmatrix} 1 \\ 1 \end{pmatrix}$$