Detailed derivation of ⟨Δx²⟩ₙ for [[Harmonic Oscillator]] energy eigenstates.
## Strategy

Calculate:
$$\langle\Delta x^2\rangle_n = \langle x^2\rangle_n - \langle x\rangle_n^2$$
## Step 1: Show ⟨x⟩ₙ = 0
From [[Ladder Operators]]:
$$\hat{x} = \sqrt{\frac{\hbar}{2m\omega}}(\hat{a} + \hat{a}^\dagger)$$

Calculate expectation value:
$$\langle x\rangle_n = \langle n|\hat{x}|n\rangle = \sqrt{\frac{\hbar}{2m\omega}}\langle n|(\hat{a} + \hat{a}^\dagger)|n\rangle$$

Using [[Lowering Operator Matrix Elements]] and [[Raising Operator Matrix Elements]]:
$$\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$$
$$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$$

Therefore:
$$\langle n|\hat{a}|n\rangle = \sqrt{n}\langle n|n-1\rangle = 0$$
$$\langle n|\hat{a}^\dagger|n\rangle = \sqrt{n+1}\langle n|n+1\rangle = 0$$

Due to orthogonality of eigenstates.

Thus:
$$\langle x\rangle_n = 0$$

## Step 2: Calculate ⟨x²⟩ₙ

$$\hat{x}^2 = \frac{\hbar}{2m\omega}(\hat{a} + \hat{a}^\dagger)^2$$

Expand:
$$\hat{x}^2 = \frac{\hbar}{2m\omega}(\hat{a}^2 + \hat{a}\hat{a}^\dagger + \hat{a}^\dagger\hat{a} + (\hat{a}^\dagger)^2)$$

## Step 3: Use Commutation Relation

From [[Ladder Operator Commutation Relation]]: [â, â†] = 1

Therefore:
$$\hat{a}\hat{a}^\dagger = \hat{a}^\dagger\hat{a} + 1 = \hat{N} + 1$$

where N̂ = â†â is the [[Number Operator]].

Substitute:
$$\hat{x}^2 = \frac{\hbar}{2m\omega}(\hat{a}^2 + \hat{N} + 1 + \hat{N} + (\hat{a}^\dagger)^2)$$

$$= \frac{\hbar}{2m\omega}(\hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1)$$

## Step 4: Evaluate Expectation Value

$$\langle n|\hat{x}^2|n\rangle = \frac{\hbar}{2m\omega}\langle n|(\hat{a}^2 + (\hat{a}^\dagger)^2 + 2\hat{N} + 1)|n\rangle$$

**Term 1**: 
$$\langle n|\hat{a}^2|n\rangle = \sqrt{n}\sqrt{n-1}\langle n|n-2\rangle = 0$$

**Term 2**: 
$$\langle n|(\hat{a}^\dagger)^2|n\rangle = \sqrt{n+1}\sqrt{n+2}\langle n|n+2\rangle = 0$$

**Term 3**: 
$$\langle n|2\hat{N}|n\rangle = 2n\langle n|n\rangle = 2n$$

**Term 4**: 
$$\langle n|1|n\rangle = 1$$

Therefore:
$$\langle x^2\rangle_n = \frac{\hbar}{2m\omega}(0 + 0 + 2n + 1) = \frac{\hbar}{2m\omega}(2n + 1)$$

## Final Result

$$\langle\Delta x^2\rangle_n = \langle x^2\rangle_n - \langle x\rangle_n^2 = \frac{\hbar}{2m\omega}(2n + 1)$$

The position uncertainty is:
$$\Delta x = \sqrt{\langle\Delta x^2\rangle_n} = \sqrt{\frac{\hbar(2n+1)}{2m\omega}}$$

## Ground State

For n = 0:
$$\langle\Delta x^2\rangle_0 = \frac{\hbar}{2m\omega}$$

This is the minimum uncertainty allowed by quantum mechanics for this system.

## Related

- [[Harmonic Oscillator Momentum Uncertainty]]
- [[Zero-Point Energy Physical Origin]]
- [[Ladder Operators]]
- [[Uncertainty]]