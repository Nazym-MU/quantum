## Problem Setup
Given:
- Particle 1: unknown state $|\psi_1\rangle = a|+z\rangle_1 + b|-z\rangle_1$
- Particles 2 & 3: entangled in [[Singlet State]] $|0,0\rangle_{23} = \frac{1}{\sqrt{2}}(|+z\rangle_2|-z\rangle_3 - |-z\rangle_2|+z\rangle_3)$
- Particle 2 goes to Alice, particle 3 to Bob

Find: what state is particle 3 in after Alice performs a [[Bell State Measurement]] on particles 1 & 2?

## Step 1: Write three-particle state

$$|\psi_{123}\rangle = |\psi_1\rangle \otimes |0,0\rangle_{23}$$

Expand explicitly:
$$= (a|+z\rangle_1 + b|-z\rangle_1) \otimes \frac{1}{\sqrt{2}}(|+z\rangle_2|-z\rangle_3 - |-z\rangle_2|+z\rangle_3)$$

$$= \frac{a}{\sqrt{2}}(|+z\rangle_1|+z\rangle_2|-z\rangle_3 - |+z\rangle_1|-z\rangle_2|+z\rangle_3) + \frac{b}{\sqrt{2}}(|-z\rangle_1|+z\rangle_2|-z\rangle_3 - |-z\rangle_1|-z\rangle_2|+z\rangle_3)$$

## Step 2: Rewrite in Bell basis

Rearrange the four terms to extract each of the four Bell states:

**Terms with $|+z\rangle_1|-z\rangle_2 - |-z\rangle_1|+z\rangle_2$:**
$$\frac{1}{2}|\Psi^-\rangle_{12} \otimes (-a|-z\rangle_3 - b|+z\rangle_3)$$

**Terms with $|+z\rangle_1|-z\rangle_2 + |-z\rangle_1|+z\rangle_2$:**
$$\frac{1}{2}|\Psi^+\rangle_{12} \otimes (-a|-z\rangle_3 + b|+z\rangle_3)$$

**Terms with $|+z\rangle_1|+z\rangle_2 + |-z\rangle_1|-z\rangle_2$:**
$$\frac{1}{2}|\Phi^+\rangle_{12} \otimes (-b|+z\rangle_3 + a|-z\rangle_3)$$

**Terms with $|+z\rangle_1|+z\rangle_2 - |-z\rangle_1|-z\rangle_2$ (sign flipped):**
$$\frac{1}{2}|\Phi^-\rangle_{12} \otimes (b|+z\rangle_3 + a|-z\rangle_3)$$

## Step 3: Complete expansion

$$|\psi_{123}\rangle = \frac{1}{2}[|\Psi^-\rangle_{12}(-a|+z\rangle_3 - b|-z\rangle_3) + |\Psi^+\rangle_{12}(-a|+z\rangle_3 + b|-z\rangle_3)$$
$$+ |\Phi^+\rangle_{12}(b|+z\rangle_3 + a|-z\rangle_3) + |\Phi^-\rangle_{12}(-b|+z\rangle_3 + a|-z\rangle_3)]$$

## Step 4: Interpret measurement outcome

When Alice measures particles 1 and 2 in the Bell basis, she projects onto one of four states with equal probability 1/4 each:

| Alice's measurement    | Particle 3's state                 | Bob's unitary correction     |
| ---------------------- | ---------------------------------- | ---------------------------- |
| $\|\Psi^-\rangle_{12}$ | $-a\|+z\rangle_3 - b\|-z\rangle_3$ | $180°$ rotation about y-axis |
| $\|\Psi^+\rangle_{12}$ | $-a\|+z\rangle_3 + b\|-z\rangle_3$ | $180°$ rotation about x-axis |
| $\|\Phi^+\rangle_{12}$ | $-b\|+z\rangle_3 + a\|-z\rangle_3$ | Swap basis + phase           |
| $\|\Phi^-\rangle_{12}$ | $b\|+z\rangle_3 + a\|-z\rangle_3$  | Different phase + basis swap |

## Key Insight
**All four outcomes leave particle 3 in a state related to the original |ψ₁⟩ by a unitary transformation.** The factors are just sign flips and basis swaps—all reversible operations. Bob applies the corresponding unitary based on Alice's 2-bit classical message to recover the original state.

The factor of 1/2 comes from normalizing: each Bell state has probability 1/4.

## Related Concepts
- [[Bell State Measurement]]
- [[Quantum Teleportation]]
- [[Singlet State]]
- [[Rotation Operators]]