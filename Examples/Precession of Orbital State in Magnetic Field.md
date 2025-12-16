Example showing how a $p_x$ orbital precesses in a magnetic field along z-axis.
Molecule initially in $p_x$ orbital, placed in magnetic field $\mathbf{B} = B_0\hat{k}$.
## Initial State (t = 0)
The $p_x$ orbital is a linear combination:
$$|\psi(0)\rangle = \frac{1}{\sqrt{2}}(|1, -1\rangle - |1, 1\rangle)$$
Angular wave function:
$$\langle\theta, \phi|\psi(0)\rangle = \sqrt{\frac{3}{4\pi}}\sin\theta\cos\phi$$
## Hamiltonian
Interaction with magnetic field:
$$\hat{H} = -\boldsymbol{\mu} \cdot \mathbf{B} = -\left(\frac{-e}{2m_ec}\hat{\mathbf{L}}\right) \cdot B_0\hat{k} = \omega_0\hat{L}_z$$
where $\omega_0 = \frac{eB_0}{2m_ec}$ is the Larmor frequency.
## Time Evolution
$$|\psi(t)\rangle = e^{-i\hat{H}t/\hbar}|\psi(0)\rangle = e^{-i\omega_0\hat{L}_z t/\hbar}|\psi(0)\rangle$$
For each eigenstate $|1, m\rangle$ with $\hat{L}_z|1, m\rangle = m\hbar|1, m\rangle$:
$$e^{-i\omega_0\hat{L}_z t/\hbar}|1, m\rangle = e^{-i\omega_0 m t}|1, m\rangle$$
## Evolved State
$$|\psi(t)\rangle = \frac{1}{\sqrt{2}}\left(e^{i\omega_0 t}|1, -1\rangle - e^{-i\omega_0 t}|1, 1\rangle\right)$$
Angular wave function:
$$\langle\theta, \phi|\psi(t)\rangle = \sqrt{\frac{3}{4\pi}}\sin\theta\cos(\phi - \omega_0 t)$$
## Physical Interpretation
The $p_x$ orbital **rotates** (precesses) about the z-axis with angular frequency $\omega_0$.
- At $t = 0$: $p_x$ orbital (along x-axis)
- At $t = T/4$ where $T = 2\pi/\omega_0$: $p_y$ orbital (along y-axis)
- At $t = T/2$: $-p_x$ orbital (along negative x-axis)
- At $t = T$: back to $p_x$ orbital
Period: $T = \frac{2\pi}{\omega_0} = \frac{4\pi m_ec}{eB_0}$
## Connection to Spin Precession
This is identical to spin precession from Chapter 4. Both spin and orbital angular momentum precess in magnetic fields. The precession frequency depends on the gyromagnetic ratio.
For orbital: $\omega_0 = \frac{eB_0}{2m_ec}$
For spin: $\omega_s = g\frac{eB_0}{2m_ec}$ where $g \approx 2$ for electron
Related: [[Cartesian Forms of Spherical Harmonics]], [[Time Evolution Operator]]
