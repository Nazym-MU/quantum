**Translational invariance**: Physics is the same regardless of absolute position in space.
Mathematically: $[Ĥ, \hat T(a)] = 0$ for any translation a.
This means translating the entire system doesn't affect energy levels or dynamics.
## Generator
Since $\hat T(a) = e^{-i\hat{P}\cdot a/ℏ}$, if the Hamiltonian commutes with translations, it must commute with the momentum operator:
$$[Ĥ, T̂(a)] = 0 ⟹ [Ĥ, P̂] = 0$$
## Conservation law
From Heisenberg equation of motion:
$$\frac{d\hat P}{dt} = \frac{i}{\hbar}[\hat H, \hat P] + \frac{\partial \hat P}{\partial t}$$
Since $\hat{P}$ has no explicit time dependence and commutator is 0, $\frac{d\hat{P}}{dt} = 0$ → momentum is conserved.
## Symmetry ↔ Conservation
- **Translational symmetry** ↔ Linear momentum conservation
- **Time translation symmetry** ↔ Energy conservation  
- **Rotational symmetry** ↔ Angular momentum conservation
## Laboratory with no windows
If you perform an experiment, then translate your entire laboratory to a different location and repeat the experiment, you get identical results. The physics doesn't depend on where you are, only on the relative configuration of objects.
Time evolution also preserves this: if |ψ(0)⟩ evolves to |ψ(t)⟩, then $\hat T(a)|ψ(0)⟩$ evolves to $\hat T(a)|ψ(t)⟩$. Translated states stay translated.
## Breaking the symmetry
External forces break translational invariance. Example: adding a third particle at fixed position r₃ makes the Hamiltonian location-dependent, so total momentum of the two-particle subsystem is no longer conserved. (However, momentum of the three-particle system remains conserved.)
Related: [[Two-Body Hamiltonian]], [[Homogeneity of Space]], [[Constants of Motion]], [[Time Evolution Operator]]
