**Rotational invariance**: Physics is the same regardless of orientation in space. Rotating the entire system doesn't affect energy levels or dynamics.
Mathematically: $[\hat H, \hat R(\theta \hat n)] = 0$ for rotations by angle $θ$ about any axis $\hat n$
## Two Methods to Verify Rotational Invariance
**Method 1: Cartesian coordinates**  
Show $[\hat H, \hat L_z] = 0$ by proving:
- $[\hat L_z, \hat p^2] = 0$ → kinetic energy invariant
- $[\hat L_z, V(r)] = 0$ → potential energy invariant

**Method 2: Spherical coordinates**  
In spherical coordinates $|r, θ, \phi⟩$:
$R̂(d\phi \hat k)|r, θ, \phi ⟩ = |r, θ, \phi + d\phi⟩$
Since V depends only on r (not on angles), $V(\hat r)$ commutes with $\hat R(d\phi \hat k)$.
## Generator Connection
Since $\hat R(θ\hat n) = e^{-i\hat L\cdot θ\hat n/ℏ}$, rotational invariance implies:
$$[Ĥ, L̂] = 0$$
## Conservation Law
From Heisenberg equation of motion:
$$\frac{d\braket \hat L}{dt} = \frac{d\braket{\psi(t) | \hat L | \psi(t)}}{dt} = \frac{i}{\hbar}\bra{\psi(t)}[\hat H, \hat L]\ket{\psi(t)} +  \braket{\psi(t) |\frac{\partial\hat L}{\partial t} |\psi(t)} = 0$$
Angular momentum is conserved.
## Applicability to All Axes
The Hamiltonian $Ĥ = p̂²/2μ + V(r)$ has no preferred direction. Therefore, the system is rotationally invariant about **any** axis.
## Symmetry ↔ Conservation
- **Rotational symmetry** ↔ Angular momentum conservation
- **Translational symmetry** ↔ Linear momentum conservation
- **Time translation symmetry** ↔ Energy conservation

Related: [[Orbital Angular Momentum as Generator of Rotations]], [[Isotropy of Space]], [[Translational Invariance and Momentum Conservation]]
