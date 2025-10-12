**Formula:** [[<6>]]
$$\frac{d}{dt}\braket{A} = \frac{i}{\hbar}\braket{[\hat{H}, \hat{A}]} + \braket{\frac{\partial \hat{A}}{\partial t}}$$
## Interpretation
The rate of change of ⟨A⟩ has two contributions:
1. **Commutator term**: (i/ℏ)⟨[Ĥ,Â]⟩ 
   - Comes from state evolution
   - Present even if  itself doesn't change
2. **Explicit time dependence**: ⟨∂Â/∂t⟩
   - Present if the operator itself changes with time
   - Example: time-varying external field
## Special Cases
**Case 1: Â commutes with Ĥ and has no explicit time dependence**
- [Ĥ,Â] = 0 and ∂Â/∂t = 0
- Result: d⟨A⟩/dt = 0
- Â is a [[Constants of Motion]]

**Case 2: Energy expectation when Ĥ is time-independent**
- [Ĥ,Ĥ] = 0 and ∂Ĥ/∂t = 0
- Result: d⟨Ĥ⟩/dt = 0 (energy conservation)

**Case 3: Superposition of energy eigenstates**
- Even if [Ĥ,Â] ≠ 0, expectation values oscillate
- Frequency determined by energy differences: ω = (E₂-E₁)/ℏ
## Related
- [[Constants of Motion]]
- [[Commutators]]
- [[Hamiltonian Operator]]