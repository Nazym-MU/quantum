Rotating ket into another ket:
$\ket{\psi'}=\hat{R}^\dagger \ket{\psi}$ 
- Acting to the right on the ket: generating a new state
- Acting to the left on the bra: transforming bases ($S_z \to S_x$)
$$\ket{\psi'} \xrightarrow[S_z \text{ basis}]{} \begin{pmatrix} \braket{+z | \psi'} \\ \braket{-z|\psi'}\end{pmatrix} = \begin{pmatrix} \braket{+z | \hat{R}^\dagger | \psi} \\ \braket{-z|\hat{R}^\dagger | \psi}\end{pmatrix} = \begin{pmatrix} \braket{+x | \psi} \\ \braket{-x | \psi}\end{pmatrix} \xleftarrow[S_x \text{ basis}]{} \ket{\psi}$$
- Left to right: active transformation (the state $\ket{\psi'}$ in the $S_z$ basis has been rotated clockwise), you can see a new state being generated in the middle
- Right to left: passive transformation (rotating the basis states counterclockwise), the state didn't change, but we transformed from $S_x$ to $S_z$
Relating $\ket{\psi}$ in $S_z$ basis to $\ket{\psi}$ in $S_x$ basis basis by inserting [[Identity operator]] [[(8)]]:
$$\begin{pmatrix} \braket{+x | \psi} \\ \braket{-x|\psi}\end{pmatrix} = \begin{pmatrix} \braket{+z | \hat{R}^\dagger\left( \frac{\pi}{2}j \right) | +z} & \braket{+z|\hat{R}^\dagger\left( \frac{\pi}{2}j \right) | -z} \\ \braket{-z|\hat{R}^\dagger\left( \frac{\pi}{2}j \right) | +z} & \braket{-z|\hat{R}^\dagger\left( \frac{\pi}{2}j \right) | -z} \end{pmatrix} \begin{pmatrix} \braket{+z | \psi} \\ \braket{-z | \psi}\end{pmatrix}$$
- $S^\dagger$ matrix in the middle (would be $S$ to convert $S_x \to S_z$):
$$\begin{pmatrix} \braket{+z | \psi} \\ \braket{-z|\psi}\end{pmatrix} = \begin{pmatrix} \braket{+z | \hat{R}\left( \frac{\pi}{2}j \right) | +z} & \braket{+z|\hat{R}\left( \frac{\pi}{2}j \right) | -z} \\ \braket{-z|\hat{R}\left( \frac{\pi}{2}j \right) | +z} & \braket{-z|\hat{R}\left( \frac{\pi}{2}j \right) | -z} \end{pmatrix} \begin{pmatrix} \braket{+x | \psi} \\ \braket{-x | \psi}\end{pmatrix}$$
$$\hat{A} \xrightarrow[S_x \text{ basis}]{} S^\dagger \mathbb{A}S, \text{ where } \mathbb{A} \text{ is the matrix representation of } \hat{A} \text{ in the } S_z \text{ basis}$$
> S matrices are composed of amplitudes formed by taking the inner product of the basis kets of the representation we're transforming from with the basis bras we're transforming to.


[[Examples Changing Representations]]

