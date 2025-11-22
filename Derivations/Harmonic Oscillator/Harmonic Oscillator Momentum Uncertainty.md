Detailed derivation of ⟨Δp²⟩ₙ for [[Harmonic Oscillator]] energy eigenstates.

## Strategy

Calculate:
$$\langle\Delta p_x^2\rangle_n = \langle p_x^2\rangle_n - \langle p_x\rangle_n^2$$

## Step 1: Show ⟨p̂ₓ⟩ₙ = 0

From [[Ladder Operators]]:
$$\hat{p}_x = -i\sqrt{\frac{m\omega\hbar}{2}}(\hat{a} - \hat{a}^\dagger)$$

Calculate expectation value:
$$\langle p_x\rangle_n = -i\sqrt{\frac{m\omega\hbar}{2}}\langle n|(\hat{a} - \hat{a}^\dagger)|n\rangle$$

Using [[Lowering Operator Matrix Elements]] and [[Raising Operator Matrix Elements]]:
$$\langle n|\hat{a}|n\rangle = \sqrt{n}\langle n|n-1\rangle = 0$$
$$\langle n|\hat{a}^\dagger|n\rangle = \sqrt{n+1}\langle n|n+1\rangle = 0$$

Therefore:
$$\langle p_x\rangle_n = 0$$

## Step 2: Calculate ⟨p̂ₓ²⟩ₙ

$$\hat{p}_x^2 = -\frac{m\omega\hbar}{2}(\hat{a} - \hat{a}^\dagger)^2$$

Expand:
$$\hat{p}_x^2 = -\frac{m\omega\hbar}{2}(\hat{a}^2 - \hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a} + (\hat{a}^\dagger)^2)$$

## Step 3: Use Commutation Relation

From [[Ladder Operator Commutation Relation]]: [â, â†] = 1

Therefore: ââ† = â†â + 1

Substitute:

$$\hat{p}_x^2 = -\frac{m\omega\hbar}{2}(\hat{a}^2 - \hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a} + (\hat{a}^\dagger)^2)$$

$$= -\frac{m\omega\hbar}{2}(\hat{a}^2 + (\hat{a}^\dagger)^2 - \hat{a}\hat{a}^\dagger - \hat{a}^\dagger\hat{a})$$

Using ââ† = N̂ + 1 and â†â = N̂:
$$= -\frac{m\omega\hbar}{2}(\hat{a}^2 + (\hat{a}^\dagger)^2 - \hat{N} - 1 - \hat{N})$$

$$= -\frac{m\omega\hbar}{2}(\hat{a}^2 + (\hat{a}^\dagger)^2 - 2\hat{N} - 1)$$

$$= \frac{m\omega\hbar}{2}(2\hat{N} + 1 - \hat{a}^2 - (\hat{a}^\dagger)^2)$$

## Step 4: Evaluate Expectation Value

$$\langle n|\hat{p}_x^2|n\rangle = \frac{m\omega\hbar}{2}\langle n|(2\hat{N} + 1 - \hat{a}^2 - (\hat{a}^\dagger)^2)|n\rangle$$

**Term 1**: 
$$\langle n|2\hat{N}|n\rangle = 2n$$

**Term 2**: 
$$\langle n|1|n\rangle = 1$$

**Term 3**: 
$$\langle n|\hat{a}^2|n\rangle = \sqrt{n}\sqrt{n-1}\langle n|n-2\rangle = 0$$

**Term 4**: 
$$\langle n|(\hat{a}^\dagger)^2|n\rangle = \sqrt{n+1}\sqrt{n+2}\langle n|n+2\rangle = 0$$

Therefore:
$$\langle p_x^2\rangle_n = \frac{m\omega\hbar}{2}(2n + 1 - 0 - 0) = \frac{m\omega\hbar}{2}(2n + 1)$$

## Final Result

$$\langle\Delta p_x^2\rangle_n = \langle p_x^2\rangle_n - \langle p_x\rangle_n^2 = \frac{m\omega\hbar}{2}(2n + 1)$$

The momentum uncertainty is:
$$\Delta p_x = \sqrt{\langle\Delta p_x^2\rangle_n} = \sqrt{\frac{m\omega\hbar(2n+1)}{2}}$$

## Ground State

For n = 0:
$$\langle\Delta p_x^2\rangle_0 = \frac{m\omega\hbar}{2}$$

## Uncertainty Product

From [[Harmonic Oscillator Position Uncertainty]]:
$$\Delta x \cdot \Delta p_x = \sqrt{\frac{\hbar(2n+1)}{2m\omega}} \cdot \sqrt{\frac{m\omega\hbar(2n+1)}{2}} = \frac{\hbar(2n+1)}{2}$$

For the ground state (n=0): Δx·Δp = ℏ/2, saturating the [[Uncertainty|Heisenberg uncertainty relation]].

## Related

- [[Harmonic Oscillator Position Uncertainty]]
- [[Zero-Point Energy Physical Origin]]
- [[Ladder Operators]]
- [[Uncertainty]]