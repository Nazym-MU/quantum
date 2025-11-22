
Explanation of why ⟨x⟩ = 0 and ⟨p⟩ = 0 for [[Harmonic Oscillator]] energy eigenstates.

## The Result

For all energy eigenstates |n⟩:
$$\langle x\rangle_n = \langle n|\hat{x}|n\rangle = 0$$
$$\langle p_x\rangle_n = \langle n|\hat{p}_x|n\rangle = 0$$

## Physical Intuition

Energy eigenstates are **stationary states**:
- Time-independent probability distributions
- Particle equally likely to be left or right of center
- Particle equally likely to move left or right
- **No net displacement, no net momentum**

The oscillator "doesn't know" which direction to prefer - it's symmetric about x = 0.

## Mathematical Proof for ⟨x⟩

### Method 1: Using Ladder Operators

From [[Ladder Operators]]:
$$\hat{x} = \sqrt{\frac{\hbar}{2m\omega}}(\hat{a} + \hat{a}^\dagger)$$

Calculate:
$$\langle n|\hat{x}|n\rangle = \sqrt{\frac{\hbar}{2m\omega}}\langle n|(\hat{a} + \hat{a}^\dagger)|n\rangle$$

From [[Raising Operator Matrix Elements]] and [[Lowering Operator Matrix Elements]]:
$$\hat{a}|n\rangle = \sqrt{n}|n-1\rangle$$
$$\hat{a}^\dagger|n\rangle = \sqrt{n+1}|n+1\rangle$$

Therefore:
$$\langle n|\hat{a}|n\rangle = \sqrt{n}\langle n|n-1\rangle = 0$$
$$\langle n|\hat{a}^\dagger|n\rangle = \sqrt{n+1}\langle n|n+1\rangle = 0$$

Both vanish due to **orthogonality** of energy eigenstates: ⟨n|m⟩ = δₙₘ.

Result:
$$\boxed{\langle x\rangle_n = 0}$$

### Method 2: Using Wave Functions

For real wave functions ψₙ(x) = ⟨x|n⟩, parity analysis:

The potential V(x) = ½mω²x² is **even**: V(-x) = V(x)

Therefore eigenfunctions have **definite parity**:
- Even states: ψₙ(-x) = ψₙ(x) for even n
- Odd states: ψₙ(-x) = -ψₙ(x) for odd n

For the expectation value:
$$\langle x\rangle = \int_{-\infty}^{\infty} x|\psi_n(x)|^2\,dx$$

The integrand x|ψₙ|² is an **odd function** (odd × even = odd for both parities).

Integral of odd function over symmetric limits:
$$\int_{-\infty}^{\infty} [\text{odd function}]\,dx = 0$$

Therefore: ⟨x⟩ = 0 ✓

## Mathematical Proof for ⟨p̂ₓ⟩

### Using Ladder Operators

From [[Ladder Operators]]:
$$\hat{p}_x = -i\sqrt{\frac{m\omega\hbar}{2}}(\hat{a} - \hat{a}^\dagger)$$

Calculate:
$$\langle n|\hat{p}_x|n\rangle = -i\sqrt{\frac{m\omega\hbar}{2}}\langle n|(\hat{a} - \hat{a}^\dagger)|n\rangle$$

Using same logic as above:
$$\langle n|\hat{a}|n\rangle = 0$$
$$\langle n|\hat{a}^\dagger|n\rangle = 0$$

Therefore:
$$\boxed{\langle p_x\rangle_n = 0}$$

## Why Non-Zero ⟨x²⟩ and ⟨p²⟩?

While averages vanish, **uncertainties do not**:

$$\langle x^2\rangle_n = \frac{\hbar}{2m\omega}(2n+1) \neq 0$$
$$\langle p_x^2\rangle_n = \frac{m\omega\hbar}{2}(2n+1) \neq 0$$

See: [[Harmonic Oscillator Position Uncertainty]], [[Harmonic Oscillator Momentum Uncertainty]]

### Why the Difference?

**x̂ and p̂ₓ**: Connect states differing by **one** quantum
- â|n⟩ ∝ |n-1⟩, â†|n⟩ ∝ |n+1⟩
- No diagonal elements: ⟨n|â|n⟩ = 0

**x̂² and p̂ₓ²**: Can connect states differing by **zero or two** quanta
- Terms like ââ† = N̂ + 1 give diagonal contribution
- ⟨n|N̂|n⟩ = n ≠ 0 (except ground state)

## Connection to Time Evolution

Since [[Stationary States|stationary states]] have time-independent expectation values:
$$\frac{d\langle x\rangle}{dt} = 0$$

But from Ehrenfest's theorem:
$$\frac{d\langle x\rangle}{dt} = \frac{\langle p_x\rangle}{m}$$

This requires ⟨pₓ⟩ = 0 for stationary states (consistent!).

Similarly:
$$\frac{d\langle p_x\rangle}{dt} = -\langle m\omega^2 x\rangle = -m\omega^2\langle x\rangle$$

This requires ⟨x⟩ = 0 for stationary states (consistent!).

## Off-Diagonal Elements

While diagonal elements vanish, **off-diagonal elements are non-zero**:
$$\langle n|\hat{x}|n\pm 1\rangle \neq 0$$
$$\langle n|\hat{p}_x|n\pm 1\rangle \neq 0$$

These enable transitions between states (e.g., absorption/emission of photons).

## Superposition States

For **coherent states** or **superpositions**, averages can be non-zero:
$$|\alpha\rangle = \sum_n c_n|n\rangle$$

These are not energy eigenstates and exhibit classical-like oscillatory motion with ⟨x⟩(t) ≠ 0.

## Summary

**In energy eigenstates**:
- ⟨x⟩ = ⟨p⟩ = 0: No preferred direction, stationary probability
- ⟨x²⟩ ≠ 0, ⟨p²⟩ ≠ 0: Particle spread over region, has momentum uncertainty
- ΔxΔp ≥ ℏ/2: Uncertainty principle satisfied

**Physical picture**: Particle "oscillates" but averages to center, with quantum uncertainty spread.

## Related

- [[Harmonic Oscillator Position Uncertainty]]
- [[Harmonic Oscillator Momentum Uncertainty]]
- [[Ladder Operators]]
- [[Stationary States]]
- [[Expectation Values]]