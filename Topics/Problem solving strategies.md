## Translation operator
Express the state as a superposition of position states $\to$ project onto position basis $\to$ use Dirac delta function
$$\braket{x|\hat T(a) |\psi} = \braket{x-a|\psi} = \psi(x-a)$$
acting on a bra, so a negative sign.
### Gaussian wave packet
Minimum uncertainty state. Gaussian wave packet $\braket{x|\psi} = Ne^{-x^2/2a} \to$ normalization condition $\to$ Gaussian integral to get the normalization constant $\to$ probability density $\to$ expectation of $x$ and $x^2 \to$ uncertainty $\to$ momentum space wave function $\to$ expectation of $p$ and $p^2 \to$ uncertainty $\to$ uncertainty relation.
### Schrödinger equation in position space
- **Time dependent**: Project the equation of motion onto position space ($\braket{x|\hat H|\psi(t)} = i\hbar\braket{x|\frac{d}{dt}|\psi(t)}$) $\to$ rewrite the left part as a sum of kinetic and potential energies $\to$ after several steps, get the time-dependent Schrödinger equation in position space (don't forget to replace the total derivative by the partial)
$$\left[ -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}+V(x)\right]\psi(x, t) = i\hbar\frac{\partial}{\partial t}\psi(x, t)$$
- **Time independent:** Take $\psi(t)$ to be an energy eigenstate (time dependence given by $\ket{E}e^{-iEt/\hbar}$) $\to$ project onto position space $\to$ replace it with a wave function $\psi_E(x, t) \to$ substitute into TDSE (equation above):
$$\left[ -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}+V(x)\right]\braket{x|E} = E\braket{x|E}$$
$$\left[ -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}+V(x)\right]\psi(x) = E\psi(x)$$
- Alternative way: eigenvalue equation $\hat H\ket E = E\ket E \to$ project onto position space
# Examples
#### [[Finite Square Well]]
$$V(x) = \begin{cases} 0 & |x| < a/2 \\ V_0 & |x| > a/2 \end{cases}$$
Rewrite the Schrödinger equation by plugging in $V_0$ and 0 and having only $\frac{d^2\psi}{dx^2}$ on the left side $\to$ replace the constants on the right with $k^2$ for the first case and $-q^2$ for the second case (you'll get $-k^2\psi$ and $q^2\psi$ on the right) $\to$ solve the differential equation and get solutions 1) $\psi(x) =A\sin kx + B \cos kx$ and 2) $\psi(x) =Ce^{qx} + De^{-qx}$ $\to$ discard the exponentials that blow up (leaves $\psi(x) =Ce^{qx}$ when $x < -a/2$ and $\psi(x) = De^{-qx}$ when $x > a/2$) $\to$ recognize that the function and its first derivative must be continuous.
#### [[Particle in a Box Solution|Particle in a box]]
$$V(x) = \begin{cases} 0 & |x| < a/2 \\ \infty & |x| > a/2 \end{cases}$$
Because of continuity, set the function at $|x|=a/2$ to 0 $\to$ express these two equations in the matrix form $\to$ for a nontrivial solution to a homogeneous set of equations, find the determinant and set it equal to 0 $\to$ find wavefunction for odd n and even n separately $\to$ find the normalization constant $\to$ recognize $k_na = n\pi$ $\to$ find energy formula:
$$E_n = \frac{\hbar^2 \pi^2 n^2}{2ma^2}$$
#### [[Bound States and Scattering Overview|Scattering in 1D]]
For unbound states, energy eigenvalues take on a continuum of values $\to$ to generate a physically acceptable state, we superpose energy solutions to form a wave packet $\to$ make the wave packet propagate to the right to project onto the potential well $\to$ particle scatters (nonzero amplitudes to be transmitted and reflected) $\to$ make a simplification (!) by treating the wave packet as a plain wave $\to$ flux of particles (somehow solves the absence of time dependence problem) as a probability current projected one by one
#### [[Probability Current]]
Find the partial of the wave function $\partial\psi(x, t)/\partial t$ $\to$ find the complex conjugate of it $\to$ find $\partial\psi^*(x, t)\psi(x, t)/\partial t \to$ express the equation in the form $\partial\psi^*(x, t)\psi(x, t)/\partial t = -\partial j_x / \partial x$, where $j_x$ is the probability current:
$$j_x = \frac{\hbar}{2mi} \left(\psi^* \frac{\partial \psi}{\partial x} -  \psi \frac{\partial \psi^*}{\partial x} \right)$$
#### [[Potential Step Scattering]]
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & x > 0 \end{cases}$$Determine the energy eigenstates, for which $\psi_E(x, t) = \psi(x)e^{-iEt/\hbar} \to$ form an eigenvalue equation for TISE $\to$ find the solutions to the left of the barrier $\to$ express the probability current for the wavefunction $\to$  separate probability current for incident and reflected parts $\to$ find the probability of reflection and transmission $\to$ find the solutions to the right of the barrier using two cases ($E > V_0$, for which the wavefunction is $Ce^{ik_0x}$, and $E<V_0$, for which the wavefunction is $Ce^{-qx}$) $\to$ express transmission and reflection probabilities in terms of $A, B,$ and $C$ $\to$ satisfy continuity (boundary conditions)
#### [[Barrier Tunneling Solution|Tunneling]]
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & 0 < x < a \\ 0 & x > a \end{cases}$$
Construct piecewise energy eigenfunction:
$$\psi(x) = \begin{cases} Ae^{ikx} + Be^{-ikx} & x < 0 \\ Fe^{qx} + Ge^{-qx} & 0 < x < a \\ Ce^{ikx} & x > a \end{cases}$$
In the middle, recognize that both rising and falling exponentials appear because the barrier is bounded $\to$ form four equations to satisfy boundary conditions $\to$ find the transmission coefficient.
## Harmonic oscillator
Determine the eigenstates and eigenvalues of the Hamiltonian $\hat H = \frac{\hat p_x^2}{2m}+\frac{1}{2}mw^2x^2$: use the commutation relation $[\hat x, \hat p_x] = i\hbar \to$ two non Hermitian operators $\hat a = \sqrt{\frac{mw}{2\hbar}}\left(\hat x + \frac{i}{mw}\hat p_x \right)$ and $\hat a^\dagger = \sqrt{\frac{mw}{2\hbar}}\left(\hat x - \frac{i}{mw}\hat p_x \right)$ $\to$ recognize the commutation relation $[a, a^\dagger] = 1 \to$ represent $\hat x$ and $\hat p$ in terms of these operators $\to$ express the Hamiltonian in terms of these $\to$ recognize that finding the eigenstates is equivalent to finding the eigenstates of the number operator $\to$ express commutation relations of $\hat N$ with $\hat a$ and $\hat a^\dagger$.
$$\hat x = \sqrt{\frac{\hbar}{2mw}}(\hat a^\dagger + \hat a) \qquad \hat p_x = i\sqrt{\frac{mw\hbar}{2}}(\hat a^\dagger - \hat a)$$
#### [[Ground State Wave Function Derivation|Ground state]] and [[Harmonic Oscillator Excited State Wave Functions|excited state wave functions]]
Determine position-space wave functions: 
Project the ground ket onto position space $\to$ get $\braket{x|\hat a|0} =\sqrt{\frac{mw}{2\hbar}}\braket{x|\left(\hat x + \frac{i}{mw}\hat p\right)|0} = 0$ $\to$ recognize momentum operator acting on a ground ket projected onto position space $\braket{x|\hat{p}_x|0}=-i\hbar\frac{\partial \braket{x|0}}{\partial x}$ $\to$ reduce the equation above to a first order differential equation $\to$ solve the equation $\to$ find the normalization constant $\to$ use $\ket{n} = \frac{(\hat a^\dagger)^n}{\sqrt{n!}}\ket{0}$ by projecting this onto position space $\to$ find the energy eigenfunctions.
#### Solving Schrödinger equation in position space
Finding energy eigenstates without ladder operators:
Project $\hat H \ket E$ onto position space, make an eigenvalue equation $\to$ get a nontrivial second-order differential equation ($-\frac{\hbar^2}{2m} \frac{d^2}{dx^2} \braket{x|E} + \frac{1}{2} mw^2x^2 \braket{x|E} = E\braket{x|E}$) $\to$ introduce a dimensionless variable $y = \sqrt{\frac{mw}{\hbar}}x$ and get the wave function $\braket{x|E}=\psi(y)$ $\to$ another dimensionless constant $\varepsilon = 2E/\hbar w$ and simplify the differential equation $\to$ take limit $|y| \to \infty$ to get rid of $\varepsilon \to$ solve the simplified differential equation $\to$ discard the exponentially increasing solution $\to$ after some steps with introducing a new variable, arrive at the power series solution $h(y) = \sum_{k=0}^{\infty} a_k y^k$, which you substitute into the differential equation for $h \to$ change of variables $k - 2 = k'$ $\to$ recognize that functions are linearly independent, and thus the only way to satisfy the equation is for $y$ to vanish $\to$ obtain two term recursion relation $\to$ infinite power series that behaves like $2/k$ for large $k$ (same behavior as $e^{y^2}$) $\to \psi \xrightarrow[|y|\to\infty]{} A y^{m} e^{y^{2}/2}$ $\to$ recognize that series must terminate $\to$ express as a polynomial in $y$ multiplied by a decreasing exponential.
### [[Radial Schrödinger Equation]]
To get the energy eigenfunctions: Project Hamiltonian onto position space $\to$ get the momentum part from orbital angular momentum (expand $\hat L^2$ from $\hat r \times \hat p$), then operators acts on states $\to$ get the position-space energy eigenvalue equation $\to$ express the radial part in terms of the momentum operator $\to$ choose simultaneous eigenstates $\to$ take only the radial part because LHS only depends on r $\to$ make a substitution of variables, introducing $u(r)$
## [[Explicit Spherical Harmonic Functions]]
Require eigenfunctions to be single-valued, so $m$ and $l$ are integers $\to$ recognize $\hat L = \hat r \times \hat p \to r \times -i\hbar \nabla \to$ express the gradient in the spherical coordinates $\to$ obtain $\hat L_x$ and $\hat L_y \to$ write the representation of $\hat L^2$ in terms of these $\to$ write the energy eigenvalue equation in position space in terms of this Laplacian $\to$ separate spherical harmonics from radial part $\to$ start with $\hat L_+ \ket{l, l} = 0 \to$ represent the raising and lowering operators in position space $\to$ solve the differential equation $\to$ normalize $\to$ apply lowering operators to find the remaining states

# Formulas 
#### [[Momentum Operator in Position Basis]]
$$\braket{x|\hat p_x|\psi} = -i\hbar \frac{\partial}{\partial x}\braket{x|\psi} \qquad \hat p_x \xrightarrow[x \text{ basis}]{}-i\hbar\frac{\partial}{\partial x}$$
#### Generator of rotations 
$$\hat R(d\phi k) = 1-\frac{i}{\hbar}\hat J_z d\phi\qquad \text{and}\qquad \hat R(\phi k) = \lim_{N\to\infty}\left[1-\frac{i}{\hbar}\hat{J}_z\frac{\phi}{N} \right]^N=e^{-i\hat{J}_z\phi/\hbar}$$
#### Generator of translations
$$\hat T(dx) = 1-\frac{i}{\hbar}\hat p_x dx\qquad \text{and}\qquad \hat T(a) = \lim_{N\to\infty}\left[1-\frac{i}{\hbar}\hat{p}_x\frac{a}{N} \right]^N=e^{-i\hat{p}_xa/\hbar}$$
#### Generator of time translations
$$\hat U(dt) = 1-\frac{i}{\hbar}\hat H dt\qquad \text{and}\qquad \hat U(t) = \lim_{N\to\infty}\left[1-\frac{i}{\hbar}\hat{H}\frac{t}{N} \right]^N=e^{-i\hat{H}t/\hbar}$$
#### Time dependence of expectation variables
$$\frac{d\braket{A}}{dt} =\frac{d}{dt}\braket{\psi(t)|\hat A|\psi(t)} =\frac{i}{\hbar} \braket{\psi(t)|[\hat H, \hat A]| \psi(t)}+\braket{\psi(t)|\frac{\partial \hat A}{\partial t}|\psi(t)}$$
$\to$ for any operator, plug it into the equation $\to$ express Hamiltonian in terms of the sum of kinetic and potential energies  $\to$ discard the commuting part $\to$ use commutator properties when needed 
$$\frac{d\braket{x}}{dt} =\frac{i}{\hbar} \braket{\psi|[\hat H, \hat x]| \psi}=\frac{\braket{{\psi |\hat p|}  \psi}}{m} \qquad \frac{d\braket{p_x}}{dt} =\frac{i}{\hbar} \braket{\psi|[\hat H, \hat p_x]| \psi}=\left\langle -\frac{dV}{dx}\right\rangle$$
### Uncertainty:
$$\Delta A \cdot \Delta B \geq \frac{|\langle C \rangle|}{2}$$where  $[\hat{A}, \hat{B}] = i\hat C$
## Actions of operators
$$\hat J^2\ket{j, m} = j(j+1) \hbar^2 \ket{j, m}$$
$$\hat J_z\ket{j, m} = m \hbar \ket{j, m}$$
$$\hat J_\pm\ket{j, m} = \sqrt{j(j+1) - m(m\pm1)}\hbar \ket{j, m\pm 1}$$
$$\hat H\ket{\psi(t)}=i\hbar \frac{d}{dt}\psi(t) \quad \leftarrow \quad \text{Schrödinger equation}$$

## Matrix representations of operators
#### Spin-1 angular momenta
$$\hat J_z = \hbar \begin{pmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & -1 \end{pmatrix}, \quad \hat J_x = \frac{\hbar}{\sqrt2} \begin{pmatrix} 0 & 1 & 0 \\ 1 & 0 & 1 \\ 0 & 1 & 0 \end{pmatrix}, \quad \hat J_y = \frac{\hbar}{\sqrt 2} \begin{pmatrix} 0 & -i & 0 \\ i & 0 & -i \\ 0 & i & 0 \end{pmatrix}, \quad \hat J^2 = 2\hbar^2 \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$$
#### Spin-1 raising and lowering
$$J^+ = \sqrt{2}\hbar \begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 0 \end{pmatrix}, \quad J^- = \sqrt{2}\hbar \begin{pmatrix} 0 & 0 & 0 \\ 1 & 0 & 0 \\ 0 & 1 & 0 \end{pmatrix}$$

## Commutation relations
