$$[\hat{A}, \hat{B}] = \hat{A}\hat{B} - \hat{B}\hat{A}$$
The commutator determines whether two observables can be simultaneously measured
## Basic Properties
1. Antisymmetry: $[\hat{A}, \hat{B}] = -[\hat{B}, \hat{A}]$
2. Linearity: $[c_1\hat{A} + c_2\hat{B}, \hat{C}] = c_1[\hat{A}, \hat{C}] + c_2[\hat{B}, \hat{C}]$
3. Product with Scalars: $[\hat{A}, c] = 0$ for any scalar c (scalars commute with everything).
4. Self-Commutator: $[\hat{A}, \hat{A}] = 0$
> Leibniz Rule [[<5>]]
> [[Why Simultaneous Eigenstates]]
> Angular momentum [[Commutation Relations]]
## Raising/Lowering Operator Commutators

$$[\hat{J}_z, \hat{J}_\pm] = \pm\hbar\hat{J}_\pm$$
where $\hat{J}_\pm = \hat{J}_x \pm i\hat{J}_y$
## Two-Particle Systems
Individual particle operators commute: $[\hat{S}_{1i}, \hat{S}_{2j}] = 0 \text{ for all } i,j$, but each particle's components don't commute: $[\hat{S}_{1x}, \hat{S}_{1y}] = i\hbar\hat{S}_{1z}$
Physical meaning: Can rotate particle 1 independently of particle 2.
## Connection to [[Uncertainty]]
The commutator appears in the uncertainty relation:
$$\Delta A \cdot \Delta B \geq \frac{1}{2}|\langle[\hat{A},\hat{B}]\rangle|$$
- Larger commutator → larger minimum uncertainty product
- $[\hat{A},\hat{B}]=0$ → can have ΔA = ΔB = 0 simultaneously
## Connection to Time Evolution
Rate of change of expectation values [[Time Dependence of Expectation Values]]:
$$\frac{d\langle A\rangle}{dt} = \frac{i}{\hbar}\langle[\hat{H}, \hat{A}]\rangle + \left\langle\frac{\partial\hat{A}}{\partial t}\right\rangle$$

If [Ĥ,Â] = 0, then ⟨Â⟩ can be a [[Constants of Motion|constant of motion]].
## [[Diagonalization]]
When $[\hat{A},\hat{B}] = 0$:
- Can be **simultaneously diagonalized**
- Choose basis of common eigenstates
- Both become diagonal matrices in that basis
When $[\hat{A},\hat{B}] ≠ 0$:
- Cannot both be diagonal in same basis
- If  is diagonal, $\hat{B}$ has off-diagonal elements (and vice versa)