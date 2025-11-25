Determine expressions for the states $|+x\rangle, |-x\rangle$ in terms of the elements of the basis $|+y\rangle, |-y\rangle$.

---
## Solution
Project $|+x\rangle, |-x\rangle$ onto the eigenbasis:
$$|+x\rangle \xrightarrow[S_y \text{ basis}]{} \langle +y|+x\rangle|+y\rangle + \langle -y|+x\rangle|-y\rangle =$$
$$= \frac{1}{2}\begin{pmatrix}1 & -i\end{pmatrix}\begin{pmatrix}1 \\ 1\end{pmatrix}|+y\rangle + \frac{1}{2}\begin{pmatrix}1 & i\end{pmatrix}\begin{pmatrix}1 \\ 1\end{pmatrix}|-y\rangle = \frac{1-i}{2}|+y\rangle + \frac{1+i}{2}|-y\rangle$$
$$|-x\rangle \xrightarrow[S_y \text{ basis}]{} \langle +y|-x\rangle|+y\rangle + \langle -y|-x\rangle|-y\rangle =$$
$$= \frac{1}{2}\begin{pmatrix}1 & -i\end{pmatrix}\begin{pmatrix}1 \\ -1\end{pmatrix}|+y\rangle + \frac{1}{2}\begin{pmatrix}1 & i\end{pmatrix}\begin{pmatrix}1 \\ -1\end{pmatrix}|-y\rangle = \frac{1+i}{2}|+y\rangle + \frac{1-i}{2}|-y\rangle$$