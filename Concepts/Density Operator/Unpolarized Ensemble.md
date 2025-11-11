# Unpolarized Ensemble

A completely unpolarized ensemble of spin-½ particles has density operator:
$$\hat{\rho} = \frac{1}{2}|+n\rangle\langle+n| + \frac{1}{2}|-n\rangle\langle-n|$$

for **any** direction n. All directions are equivalent.

## Matrix Representation
In any basis (e.g., Sᵤ basis):
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = \frac{1}{2}\hat{I}$$

## Properties
**Isotropy**: Same density operator for any spin direction n
- 50% |+z⟩, 50% |-z⟩
- 50% |+x⟩, 50% |-x⟩  
- 50% |+y⟩, 50% |-y⟩
- All give ρ = (1/2)I

**Expectation values**: All vanish
$$\langle\hat{S}_x\rangle = \langle\hat{S}_y\rangle = \langle\hat{S}_z\rangle = 0$$

**Measurements**: Equal probability for any direction
$$P(+n) = P(-n) = \frac{1}{2}$$
for any direction n.

## Mixed State Properties
- tr ρ = 1 ✓
- tr ρ² = 1/2 < 1 → mixed state
- No off-diagonal elements (no coherence)

## Physical Examples
**Original Stern-Gerlach Experiment**: Silver atoms from oven exit unpolarized—no preferred spin direction.

**High Temperature Limit**: For μB/kᴮT ≪ 1, thermal ensemble becomes ρ → (1/2)I.

## Comparison: Unpolarized vs Pure States
| State | Density Operator | ⟨Sᵤ⟩ | tr ρ² |
|-------|-----------------|-------|-------|
| Unpolarized | (1/2)I | 0 | 1/2 |
| \|+z⟩ | \|+z⟩⟨+z\| | ℏ/2 | 1 |
| \|+x⟩ | \|+x⟩⟨+x\| | 0 | 1 |

Note: |+x⟩ has ⟨Sᵤ⟩ = 0 but is **not** unpolarized—it's a pure state with ⟨Sₓ⟩ = ℏ/2.

## Non-Uniqueness of Preparation
Cannot determine preparation method from ρ = (1/2)I. Could be:
- Atoms from oven (random thermal motion)
- 50-50 mix from SGz filter
- 50-50 mix from SGx filter
- Any other 50-50 split along any axis

**All are the same quantum state** because ρ is identical → identical predictions for all measurements.

## Related
- [[Density Operator Mixed State]]
- [[Thermal Equilibrium and Density Operator]]
- [[The original Stern-Gerlach Experiment]]
- [[Off-Diagonal Elements and Coherence]]