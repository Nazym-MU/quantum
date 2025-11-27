Consider the matrix representation from the previous breakout.
$$\begin{bmatrix}E_1 & 0 & E_{13} \\ 0 & E_2 & 0 \\ E_{13} & 0 & E_1 \end{bmatrix}$$
$$\psi(t)=\hat U(t)\ket{\psi(0)}=e^{-i\hat H t/\hbar}\ket{\psi(0)}$$

---
Suppose the initial state of our three-state system is $\ket{\psi(0)} =\ket{2}$. What does it become at some later time t?

There is only one nonzero entry at position (2, 2), so it's an eigenstate of $\hat H$. 
$$\hat H\ket2 = E_2\ket2$$
$$\ket{\psi(t)}=e^{-iE_2t/\hbar}$$ picks up a global phase.

---
Suppose the initial state of our three-state system is $\ket{\psi(0)} =\ket{3}$. What does it become at some later time t?
Not an eigenstate because superposition of energy eigenstates.
#### 1) Find the eigenvalues in the $\{|1\rangle, |3\rangle\}$ subspace:
$$\hat{H} = \begin{bmatrix} E_1 & E_{13} \\ E_{13} & E_1 \end{bmatrix}$$
$$\det\begin{bmatrix} E_1 - \lambda & E_{13} \\ E_{13} & E_1 - \lambda \end{bmatrix} = (E_1 - \lambda)^2 - E_{13}^2 = 0$$
$$\lambda = E_1 \pm E_{13}$$
#### 2) Find the eigenvectors:
**For $\lambda_+ = E_1 + E_{13}$:**
$$\begin{bmatrix} -E_{13} & E_{13} \\ E_{13} & -E_{13} \end{bmatrix}\begin{bmatrix} v_1 \\ v_2 \end{bmatrix} = 0$$
$$-E_{13}v_1 + E_{13}v_2 = 0$$
$$v_1 = v_2$$
$$|+\rangle = \frac{1}{\sqrt{2}}(|1\rangle + |3\rangle)$$
**For $\lambda_- = E_1 - E_{13}$:**
$$E_{13}v_1 + E_{13}v_2 = 0$$
$$v_1 = -v_2$$
$$|-\rangle = \frac{1}{\sqrt{2}}(|1\rangle - |3\rangle)$$
#### 3) Express $|3\rangle$ in eigenstate basis:

$$|3\rangle = \frac{1}{\sqrt{2}}|+\rangle - \frac{1}{\sqrt{2}}|-\rangle$$
### 4) Apply time evolution:
$$|\psi(t)\rangle = \frac{1}{\sqrt{2}}e^{-i(E_1 + E_{13})t/\hbar}|+\rangle - \frac{1}{\sqrt{2}}e^{-i(E_1 - E_{13})t/\hbar}|-\rangle$$
$$= \frac{1}{2}e^{-i(E_1 + E_{13})t/\hbar}(|1\rangle + |3\rangle) - \frac{1}{2}e^{-i(E_1 - E_{13})t/\hbar}(|1\rangle - |3\rangle)$$
$$= \frac{1}{2}e^{-iE_1 t/\hbar}\left[\left(e^{-iE_{13}t/\hbar} - e^{iE_{13}t/\hbar}\right)|1\rangle + \left(e^{-iE_{13}t/\hbar} + e^{iE_{13}t/\hbar}\right)|3\rangle\right]$$
Using $e^{ix} - e^{-ix} = 2i\sin x$ and $e^{ix} + e^{-ix} = 2\cos x$:
$$= e^{-iE_1 t/\hbar}\left[-i\sin\left(\frac{E_{13}t}{\hbar}\right)|1\rangle + \cos\left(\frac{E_{13}t}{\hbar}\right)|3\rangle\right]$$
$$\boxed{|\psi(t)\rangle = e^{-iE_1 t/\hbar}\left[-i\sin\left(\frac{E_{13}t}{\hbar}\right)|1\rangle + \cos\left(\frac{E_{13}t}{\hbar}\right)|3\rangle\right]}$$