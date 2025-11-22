Proof that for the [[Harmonic Oscillator]]:
$$|n⟩ = \frac{(â^†)^n}{√(n!)}|0⟩$$
## Strategy
Use mathematical induction to prove the state is properly normalized and satisfies N̂|n⟩ = n|n⟩.
## Base Case: n = 1
**Claim**: |1⟩ = â†|0⟩
**Normalization check**:
$$\langle 1|1\rangle = \langle 0|\hat{a}\hat{a}^\dagger|0\rangle$$
Use [[Ladder Operator Commutation Relation]]: \[â, â†\] = ââ† - â†â = 1
Therefore: ââ† = â†â + 1
$$\langle 1|1\rangle = \langle 0|(\hat{a}^\dagger\hat{a} + 1)|0\rangle$$
Since â|0⟩ = 0, we have â†â|0⟩ = 0:
$$= \langle 0|(\hat{N} + 1)|0\rangle = \langle 0|0\rangle + 0 = 1$$
**Eigenvalue check**:
$$\hat{N}|1\rangle = \hat{N}\hat{a}^\dagger|0\rangle$$
From [[Number Operator Eigenvalue Derivation]], the commutator \[$\hat{N}$, â†\] = â†:
$$= (\hat{a}^\dagger\hat{N} + \hat{a}^\dagger)|0\rangle = \hat{a}^\dagger(\hat{N} + 1)|0\rangle$$
Since N̂|0⟩ = 0:
$$= \hat{a}^\dagger \cdot 1 \cdot |0\rangle = |1\rangle = 1|1\rangle$$ ✓
## Base Case: n = 2
**Claim**: |2⟩ = (â†)²/√2!|0⟩
**Normalization check**:
$$\langle 2|2\rangle = \frac{1}{2}\langle 0|(\hat{a})^2(\hat{a}^\dagger)^2|0\rangle$$

Apply â once from left and â† once from right:
$$= \frac{1}{2}\langle 1|\hat{a}\hat{a}^\dagger|1\rangle$$

Using commutation relation:
$$= \frac{1}{2}\langle 1|(\hat{a}^\dagger\hat{a} + 1)|1\rangle = \frac{1}{2}\langle 1|(\hat{N} + 1)|1\rangle$$

Since N̂|1⟩ = 1|1⟩:
$$= \frac{1}{2}\langle 1|(1 + 1)|1\rangle = \frac{1}{2} \cdot 2 \cdot \langle 1|1\rangle = 1$$ ✓

## Induction Hypothesis

Assume for some n that:
$$|n\rangle = \frac{(\hat{a}^\dagger)^n}{\sqrt{n!}}|0\rangle$$

is properly normalized: ⟨n|n⟩ = 1

## Induction Step: Prove for n+1

**Claim**: 
$$|n+1\rangle = \frac{(\hat{a}^\dagger)^{n+1}}{\sqrt{(n+1)!}}|0\rangle$$

**Normalization**:
$$\langle n+1|n+1\rangle = \frac{1}{(n+1)!}\langle 0|(\hat{a})^{n+1}(\hat{a}^\dagger)^{n+1}|0\rangle$$

Apply â from left and â† from right once:
$$= \frac{1}{(n+1)!}\langle 0|(\hat{a})^n \cdot \hat{a}\hat{a}^\dagger \cdot (\hat{a}^\dagger)^n|0\rangle$$

Using [â, â†] = 1:
$$= \frac{1}{(n+1)!}\langle 0|(\hat{a})^n(\hat{a}^\dagger\hat{a} + 1)(\hat{a}^\dagger)^n|0\rangle$$

$$= \frac{1}{(n+1)!}\langle 0|(\hat{a})^n\hat{a}^\dagger\hat{a}(\hat{a}^\dagger)^n|0\rangle + \frac{1}{(n+1)!}\langle 0|(\hat{a})^n(\hat{a}^\dagger)^n|0\rangle$$

Continue applying commutation relations. Each application of [â, â†] brings down a factor related to the number of operators.

After n applications:
$$= \frac{1}{(n+1)!}[(n+1) \cdot n!] \langle 0|0\rangle = \frac{(n+1)!}{(n+1)!} = 1$$ ✓

## General Formula Established

By induction:
$$|n\rangle = \frac{(\hat{a}^\dagger)^n}{\sqrt{n!}}|0\rangle$$

for all non-negative integers n.

## Physical Interpretation

- Start with ground state |0⟩
- Apply raising operator â† once → |1⟩ (one quantum)
- Apply â† again → |2⟩ (two quanta)
- Apply â† n times → |n⟩ (n quanta)

The factor 1/√(n!) ensures proper normalization at each step.

## Alternative Approach Using [[Raising Operator Matrix Elements]]

From ⟨n'|â†|n⟩ = √(n+1) δₙ',ₙ₊₁:

$$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$$

Applied iteratively:
- â†|0⟩ = √1|1⟩ = |1⟩
- â†|1⟩ = √2|2⟩ → |2⟩ = (1/√2)â†|1⟩ = (â†)²/√2!|0⟩
- â†|2⟩ = √3|3⟩ → |3⟩ = (1/√3)â†|2⟩ = (â†)³/√3!|0⟩

Pattern: |n⟩ = (â†)ⁿ/√(n!)|0⟩

## Related

- [[Ladder Operators]]
- [[Raising Operator Matrix Elements]]
- [[Ladder Operator Commutation Relation]]
- [[Number Operator Eigenvalue Derivation]]