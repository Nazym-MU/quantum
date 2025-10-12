Probability weighted average of observable measured over many identically prepared systems:
$$\langle\hat{A}\rangle = \langle\psi|\hat{A}|\psi\rangle$$
## Physical Interpretation
- NOT the value of a single measurement (which is always an eigenvalue)
- Average over many measurements on identically prepared states
- Requires statistically significant sample (~ √N measurements)
## Calculation in Terms of Eigenvalues
If $|\psi\rangle = \sum_n c_n|a_n\rangle$ where Â|aₙ⟩ = aₙ|aₙ⟩: $\langle\hat{A}\rangle = \sum_n |c_n|^2 a_n$
When in an eigenstate, expectation value equals the eigenvalue (100% certainty).
In a given basis:
$$\langle\hat{A}\rangle = \begin{pmatrix} c_+^* & c_-^* \end{pmatrix} \begin{pmatrix} A_{++} & A_{+-} \\ A_{-+} & A_{--} \end{pmatrix} \begin{pmatrix} c_+ \\ c_- \end{pmatrix} = c_+^* c_+ A_{++} + c_+^* c_- A_{+-} + c_-^* c_+ A_{-+} + c_-^* c_- A_{--}$$
## Properties
- Real for Hermitian operators: $\langle\hat{A}\rangle^* = \langle\psi|\hat{A}|\psi\rangle^* = \langle\psi|\hat{A}^\dagger|\psi\rangle = \langle\psi|\hat{A}|\psi\rangle = \langle\hat{A}\rangle$
- Bounded by eigenvalues: $a_{\text{min}} \leq \langle\hat{A}\rangle \leq a_{\text{max}}$
- Linearity: $\langle c_1\hat{A} + c_2\hat{B}\rangle = c_1\langle\hat{A}\rangle + c_2\langle\hat{B}\rangle$

Used to calculate [[Uncertainty]]: $\Delta A = \sqrt{\langle\hat{A}^2\rangle - \langle\hat{A}\rangle^2}$
## Time Dependence
For time-dependent states |ψ(t)⟩: $\langle\hat{A}\rangle(t) = \langle\psi(t)|\hat{A}|\psi(t)\rangle$
- Rate of change: [[Time Dependence of Expectation Values]]
$$\frac{d}{dt}\langle A\rangle = \frac{i}{\hbar}\langle[\hat{H}, \hat{A}]\rangle + \left\langle\frac{\partial \hat{A}}{\partial t}\right\rangle$$
- If [Ĥ,Â] = 0 and ∂Â/∂t = 0, then ⟨Â⟩ is a [[Constants of Motion|constant of motion]].
## Difference Between Bases
The expectation value is **basis-independent** (it's a physical observable):
$$\langle\hat{A}\rangle = \langle\psi|\hat{A}|\psi\rangle$$
## Important Cases
- [[Stationary States]]: For energy eigenstates, all expectation values are time-independent:
$$|\psi(t)\rangle = e^{-iEt/\hbar}|E\rangle$$
$$\langle\hat{A}\rangle(t) = \langle E|e^{iEt/\hbar}\hat{A}e^{-iEt/\hbar}|E\rangle = \langle E|\hat{A}|E\rangle$$
- Superposition States:
$$|\psi(t)\rangle = c_1 e^{-iE_1t/\hbar}|E_1\rangle + c_2 e^{-iE_2t/\hbar}|E_2\rangle$$
Expectation values **oscillate** with frequency ω = (E₂ - E₁)/ℏ due to relative phase evolution.
## Related
- [[Uncertainty]]
- [[Quantum States and Amplitudes]]
- [[Measurement and State Collapse]]
- [[Time Dependence of Expectation Values]]
- [[Hermitian Operators]]