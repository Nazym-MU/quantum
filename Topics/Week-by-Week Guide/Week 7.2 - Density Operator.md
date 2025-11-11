- **Pure vs Mixed States**
	- Pure state: System is definitely in state |ψ⟩
	- Mixed state: System is in state |ψₖ⟩ with probability pₖ (classical uncertainty)
- **Density Operator Formalism**
	- Unifies treatment of pure and mixed states
	- Enables calculation of expectation values and probabilities
	- Distinguishes quantum superposition from classical statistical mixture
- **Trace Conditions**
	- tr ρ = 1 (normalization)
	- tr ρ² = 1 for pure states
	- tr ρ² < 1 for mixed states (test for mixedness)
## Key Concepts
- [[Density Operator Pure State]]
- [[Density Operator Mixed State]]
- [[Trace of Density Operator]]
- [[Expectation Values from Density Operator]]
- [[Off-Diagonal Elements and Coherence]]
## Key Results
- Different preparation methods → same density operator → same quantum state
- Off-diagonal matrix elements encode quantum coherence (relative phase)
- Density operator for projection: ρ = |ψ⟩⟨ψ| (projection operator)
- Time evolution: iℏ(dρ/dt) = \[Ĥ, ρ]
## Mathematical Tools
- Trace: $tr(ρ_ = \sum_i ⟨i|ρ|i⟩$ (basis-independent)
- Cyclic property: tr(AB) = tr(BA)
- Hermiticity: $ρ^\dagger = ρ (ρ_{i, j} = ρ_{j, i}^*)$
- Completeness: $\sum_i |i⟩⟨i| = I$