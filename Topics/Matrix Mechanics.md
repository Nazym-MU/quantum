$$|\psi\rangle \xrightarrow[\text{S}_z \text{ basis}]{} \begin{pmatrix} \braket{+z | \psi} \\ \braket{-z | \psi} \end{pmatrix} = \begin{pmatrix} c_+ \\ c_- \end{pmatrix} \qquad \langle\psi| \xrightarrow[\text{S}_z \text{ basis}]{} \begin{pmatrix} \braket{\psi | +z} & \braket{\psi | -z} \end{pmatrix} = \begin{pmatrix} c_+^* & c_-^* \end{pmatrix}$$
$$|+z\rangle \xrightarrow[\text{S}_z \text{ basis}]{} \begin{pmatrix} \braket{+z | +z} \\ \braket{-z | +z} \end{pmatrix} = \begin{pmatrix} 1 \\ 0 \end{pmatrix} \qquad |-z\rangle \xrightarrow[\text{S}_z \text{ basis}]{} \begin{pmatrix} \braket{+z | -z} \\ \braket{-z | -z} \end{pmatrix} = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$$ 
$$| +x \rangle \xrightarrow[\text{S}_z \text{ basis}]{}  \frac{e^{-i\delta}}{\sqrt{2}} \begin{pmatrix}  1 \\ 1  \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ 1 \end{pmatrix} \qquad | -x \rangle \xrightarrow[\text{S}_z \text{ basis}]{} \frac{e^{i\delta}}{\sqrt{2}} \begin{pmatrix} 1 \\ -1 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -1 \end{pmatrix}$$
$$| +y \rangle \xrightarrow[\text{S}_z \text{ basis}]{} \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ i \end{pmatrix} \qquad | -y \rangle \xrightarrow[\text{S}_z \text{ basis}]{} \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -i \end{pmatrix}$$
- [[Rotation operator]]: [[Rotation Matrix Representation]]
- [[Identity operator]]: 
- [[Projection operator]]: [[Projection Matrix Representation]]
- [[Changing Representations]]
- [[Expectation value]]: [[Expectation Value Matrix Representation]]
Matrix representation of the equation $\hat{A} \ket{\psi} = \ket{\phi}$ expressed through z basis projected onto z bases:
$$\begin{pmatrix} \braket{+z | \hat{A} | +z} &&  \braket{+z | \hat{A} | -z} \\ \braket{-z | \hat{A} | +z} && \braket{-z | \hat{A} | -z} \end{pmatrix}\begin{pmatrix} \braket{+z | \psi}  \\ \braket{-z | \psi} \end{pmatrix} = \begin{pmatrix} \braket{+z | \phi}  \\ \braket{-z | \phi} \end{pmatrix}$$

$\hat{A}$ is the operator. Bras are rows and kets are columns. 
Matrix $\hat{A}^\dagger$ is the transpose conjugate of $\hat{A}$ for all [[Hermitian operator]]s.
