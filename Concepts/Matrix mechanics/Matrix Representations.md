$$|+z\rangle \xrightarrow[\text{S}_z \text{ basis}]{} \begin{pmatrix} \braket{+z | +z} \\ \braket{-z | +z} \end{pmatrix} = \begin{pmatrix} 1 \\ 0 \end{pmatrix} \qquad |-z\rangle \xrightarrow[\text{S}_z \text{ basis}]{} \begin{pmatrix} \braket{+z | -z} \\ \braket{-z | -z} \end{pmatrix} = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$$ 
$$| +x \rangle \xrightarrow[\text{S}_z \text{ basis}]{}  \frac{e^{-i\delta}}{\sqrt{2}} \begin{pmatrix}  1 \\ 1  \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ 1 \end{pmatrix} \qquad | -x \rangle \xrightarrow[\text{S}_z \text{ basis}]{} \frac{e^{i\delta}}{\sqrt{2}} \begin{pmatrix} 1 \\ -1 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -1 \end{pmatrix}$$
$$| +y \rangle \xrightarrow[\text{S}_z \text{ basis}]{} \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ i \end{pmatrix} \qquad | -y \rangle \xrightarrow[\text{S}_z \text{ basis}]{} \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -i \end{pmatrix}$$
## States as Vectors
In basis {|a₁⟩, |a₂⟩, ...}:
$$|\psi\rangle \rightarrow \begin{pmatrix} \langle a_1|\psi\rangle \\ \langle a_2|\psi\rangle \\ \vdots \end{pmatrix} \qquad \langle\psi| \rightarrow \begin{pmatrix} \langle\psi|a_1\rangle & \langle\psi|a_2\rangle & \cdots \end{pmatrix}$$

## Operators as Matrices
Operator  in basis {|aᵢ⟩}:
$$\hat{A} \rightarrow \text{Matrix with elements } A_{ij} = \langle a_i|\hat{A}|a_j\rangle$$
$$\mathbb{A} = \begin{pmatrix} \langle a_1|\hat{A}|a_1\rangle & \langle a_1|\hat{A}|a_2\rangle & \cdots \\ \langle a_2|\hat{A}|a_1\rangle & \langle a_2|\hat{A}|a_2\rangle & \cdots \\ \vdots & \vdots & \ddots \end{pmatrix}$$
Operator is diagonal in its **eigenbasis**:
$$\hat{A}|a_n\rangle = a_n|a_n\rangle \implies \mathbb{A} = \begin{pmatrix} a_1 & 0 & \cdots \\ 0 & a_2 & \cdots \\ \vdots & \vdots & \ddots \end{pmatrix}$$
> [[Computing Matrix Elements]]
---
## Operator Actions
Equation $\hat{A}|\psi\rangle = |\phi\rangle$ becomes:
$$\mathbb{A} \begin{pmatrix} \langle a_1|\psi\rangle \\ \vdots \end{pmatrix} = \begin{pmatrix} \langle a_1|\phi\rangle \\ \vdots \end{pmatrix}$$
## Expectation Values
$$\langle\hat{A}\rangle = \langle\psi|\hat{A}|\psi\rangle = \begin{pmatrix} \psi_1^* & \psi_2^* \end{pmatrix} \begin{pmatrix} A_{11} & A_{12} \\ A_{21} & A_{22} \end{pmatrix} \begin{pmatrix} \psi_1 \\ \psi_2 \end{pmatrix}$$
## Basis Transformations
To change from basis {|aᵢ⟩} to {|bᵢ⟩}:
$$\mathbb{A}_{\text{new}} = S^\dagger \mathbb{A}_{\text{old}} S$$
where S is transformation matrix: $S_{ij} = \langle a_i|b_j\rangle$
## Related
- [[Spin Operators (Pauli Matrices)]]
- [[Euler Formula and Complex Numbers]]