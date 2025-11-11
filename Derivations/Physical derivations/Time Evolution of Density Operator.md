# Time Evolution of Density Operator

Derivation of density operator time evolution from Schrödinger equation.

## Starting Point
Schrödinger equation:
$$i\hbar\frac{\partial}{\partial t}|\psi(t)\rangle = \hat{H}|\psi(t)\rangle$$

Hermitian conjugate:
$$-i\hbar\frac{\partial}{\partial t}\langle\psi(t)| = \langle\psi(t)|\hat{H}$$

## For Pure State
Density operator: ρ̂(t) = |ψ(t)⟩⟨ψ(t)|

Time derivative:
$$\frac{d\hat{\rho}}{dt} = \frac{d}{dt}\left(|\psi(t)\rangle\langle\psi(t)|\right)$$

Using product rule:
$$\frac{d\hat{\rho}}{dt} = \left(\frac{\partial}{\partial t}|\psi(t)\rangle\right)\langle\psi(t)| + |\psi(t)\rangle\left(\frac{\partial}{\partial t}\langle\psi(t)|\right)$$

Substitute Schrödinger equation:
$$\frac{d\hat{\rho}}{dt} = \frac{1}{i\hbar}\hat{H}|\psi(t)\rangle\langle\psi(t)| + |\psi(t)\rangle\langle\psi(t)|\frac{1}{(-i\hbar)}\hat{H}$$

$$= \frac{1}{i\hbar}\hat{H}\hat{\rho} - \frac{1}{i\hbar}\hat{\rho}\hat{H}$$

$$= \frac{1}{i\hbar}[\hat{H}, \hat{\rho}]$$

Therefore:
$$i\hbar\frac{d\hat{\rho}}{dt} = [\hat{H}, \hat{\rho}]$$

## For Mixed State
For ρ̂ = Σₖ pₖ|ψₖ(t)⟩⟨ψₖ(t)|, where pₖ are time-independent probabilities:

$$\frac{d\hat{\rho}}{dt} = \sum_k p_k \frac{d}{dt}\left(|\psi_k(t)\rangle\langle\psi_k(t)|\right)$$

Each term evolves like pure state:
$$\frac{d\hat{\rho}}{dt} = \sum_k p_k \frac{1}{i\hbar}[\hat{H}, |\psi_k\rangle\langle\psi_k|]$$

$$= \frac{1}{i\hbar}\left[\hat{H}, \sum_k p_k|\psi_k\rangle\langle\psi_k|\right] = \frac{1}{i\hbar}[\hat{H}, \hat{\rho}]$$

## Von Neumann Equation
$$i\hbar\frac{d\hat{\rho}}{dt} = [\hat{H}, \hat{\rho}]$$

This is the **quantum Liouville equation** or **von Neumann equation**.

Analogous to classical Liouville equation for phase space probability density.

## Properties
**Hermiticity preserved**: If ρ̂(0) is Hermitian, then ρ̂(t) is Hermitian for all t.

**Trace preserved**: 
$$\frac{d}{dt}\text{tr}(\hat{\rho}) = \text{tr}\left(\frac{d\hat{\rho}}{dt}\right) = \frac{1}{i\hbar}\text{tr}([\hat{H}, \hat{\rho}]) = 0$$
Since tr([Â,B̂]) = 0 always.

**Purity preserved**: tr(ρ̂²) is constant in time.
- Pure states remain pure
- Mixed states remain mixed

## Formal Solution
For time-independent Ĥ:
$$\hat{\rho}(t) = \hat{U}(t)\hat{\rho}(0)\hat{U}^\dagger(t)$$

where Û(t) = e^(-iĤt/ℏ) is the [[Time Evolution Operator]].

## Related
- [[Schrödinger Equation (Time-Dependent)]]
- [[Time Evolution Operator]]
- [[Hamiltonian Operator]]
- [[Density Operator Pure State]]