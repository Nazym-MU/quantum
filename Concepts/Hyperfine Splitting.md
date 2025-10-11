The splitting of atomic energy levels due to the interaction between the magnetic moments of the nucleus and the electrons. In hydrogen, this is the interaction between the proton's and electron's magnetic moments.
## Physical Origin
- Proton has a magnetic moment → creates a magnetic field
- Electron's magnetic moment interacts with this field
- Energy depends on the **relative orientation** of the two spins
## The Hamiltonian (Hydrogen Ground State)
Matrix representation -> [[(15)]]
For ℓ = 0 states (zero orbital angular momentum): $$\hat{H}_{\text{hf}} = \frac{2A}{\hbar^2}\hat{S}_1 \cdot \hat{S}_2$$
where:
- $\hat{S}_1$ = electron spin operator
- $\hat{S}_2$ = proton spin operator
- $A$ > 0 = coupling constant (energy), determined experimentally
- Factor $\hbar^2$ ensures correct dimensions
## Energy Level Structure
The ground state energy $E_1$ splits into **two levels**:
-  Singlet State (Total Spin S = 0)
	- **Energy:** $E = E_1 - \frac{3A}{2}$ (ground state, lower energy)
	- **State:** $\frac{1}{\sqrt{2}}(|+z, -z\rangle - |-z, +z\rangle)$
	- Spins are **antiparallel** (opposite directions)
	- 1 state (non-degenerate)
	- Antisymmetric under particle exchange
- Triplet State (Total Spin S = 1)
	- **Energy:** $E = E_1 + \frac{A}{2}$ (excited state, higher energy)
	- **States:**
		- $|+z, +z\rangle$ (both up)
		- $\frac{1}{\sqrt{2}}(|+z, -z\rangle + |-z, +z\rangle)$ (symmetric superposition)
		- $|-z, -z\rangle$ (both down)
	- Spins can be **parallel** or in symmetric superposition
### Energy Difference
$$\Delta E = \frac{A}{2} - \left(-\frac{3A}{2}\right) = 2A$$
### Transition Properties
Photon emitted/absorbed when transitioning between singlet and triplet: $$h\nu = 2A$$
## Connection to Total Angular Momentum
The eigenstates are also eigenstates of **total spin**: $$\hat{S}_{\text{total}} = \hat{S}_1 + \hat{S}_2$$
- Singlet: $S = 0$, $m_S = 0$ (one state)
- Triplet: $S = 1$, $m_S \in {-1, 0, +1}$ (three states)
The Hamiltonian can be rewritten: $$\hat{H} \propto \hat{S}_1 \cdot \hat{S}_2 = \frac{1}{2}[\hat{S}^2_{\text{total}} - \hat{S}^2_1 - \hat{S}^2_2]$$
This shows energy depends on total spin.