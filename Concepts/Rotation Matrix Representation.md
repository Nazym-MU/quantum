$\hat{J}_z$ matrix representation ([[Rotation operator]])

$$\hat{J}_z \xrightarrow[S_z\text{ basis}]{} \begin{pmatrix} \braket{+z | \hat{J}_z | +z} &&  \braket{+z | \hat{J}_z | -z} \\ \braket{-z | \hat{J}_z | +z} && \braket{-z | \hat{J}_z | -z} \end{pmatrix} = \begin{pmatrix} \frac{\hbar}{2}\braket{+z | +z} &&  -\frac{\hbar}{2}\braket{+z | -z} \\ \frac{\hbar}{2}\braket{-z | +z} && -\frac{\hbar}{2}\braket{-z |  -z} \end{pmatrix} = \begin{pmatrix} \frac{\hbar}{2} &&  0 \\ 0 && -\frac{\hbar}{2} \end{pmatrix}$$
Diagonal matrix with eigenstates as basis.
$\hat{J}_z$ acting on (1, 0) and (0, 1) eigenvectors:
$$\begin{pmatrix} h/2 & 0 \\ 0 & -h/2 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \frac{h}{2} \begin{pmatrix} 1 \\ 0 \end{pmatrix} \qquad \begin{pmatrix} h/2 & 0 \\ 0 & -h/2 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = -\frac{h}{2} \begin{pmatrix} 0 \\ 1 \end{pmatrix}$$

So $\pm \frac{\hbar}{2}$ are the eigenvalues.
With projection matrices:
$$\hat{j}_z \xrightarrow[S_z \text{ basis}]{} \begin{pmatrix} \hbar/2 & 0 \\ 0 & -\hbar/2 \end{pmatrix} = \frac{\hbar}{2}\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} - \frac{\hbar}{2}\begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix}$$
$$\hat{j}_z = \frac{\hbar}{2}\hat{P}_+ - \frac{\hbar}{2}\hat{P}_- = \frac{\hbar}{2}|+z\rangle\langle+z| - \frac{\hbar}{2}|-z\rangle\langle-z|$$