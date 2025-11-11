## Statement
It is impossible to create a unitary operator U that clones an arbitrary quantum state. That is, there is no unitary U such that:
$$U|\psi\rangle|e\rangle = |\psi\rangle|\psi\rangle$$
$$U|\phi\rangle|e\rangle = |\phi\rangle|\phi\rangle$$
for all states |ψ⟩ and |φ⟩, where |e⟩ is a blank state.

## Derivation

**Step 1: Take inner product of initial states**

Start with the two initial states and take their inner product:
$$\langle\psi|_1\langle e|_2 |\phi\rangle_1|e\rangle_2 = \langle\psi|\phi\rangle \cdot \langle e|e\rangle = \langle\psi|\phi\rangle$$

**Step 2: Insert U†U (identity for unitary U)**

$$\langle\psi|_1\langle e|_2 U^\dagger U |\phi\rangle_1|e\rangle_2 = \langle\psi|\phi\rangle$$

**Step 3: Apply the cloning requirement**

Since U is supposed to clone both states:
- $U|\psi\rangle|e\rangle = |\psi\rangle|\psi\rangle$, so $U^\dagger U|\psi\rangle|e\rangle = |\psi\rangle|\psi\rangle$
- $U|\phi\rangle|e\rangle = |\phi\rangle|\phi\rangle$, so $(U|\phi\rangle|e\rangle)^\dagger = \langle\phi|\langle\phi|$

Therefore:
$$\langle\psi|\langle\psi| U^\dagger U |\phi\rangle|\phi\rangle = \langle\psi|\phi\rangle$$

**Step 4: Evaluate**

$$\langle\psi|\phi\rangle \cdot \langle\psi|\phi\rangle = \langle\psi|\phi\rangle$$

$$\langle\psi|\phi\rangle^2 = \langle\psi|\phi\rangle$$

**Step 5: Reach contradiction**

Let $x = \langle\psi|\phi\rangle$. Then $x^2 = x$, which means:
$$x(x-1) = 0$$

So either $x = 0$ or $x = 1$, meaning:
- $|\psi\rangle = |\phi\rangle$ (identical states), or
- $\langle\psi|\phi\rangle = 0$ (orthogonal states)

For arbitrary |ψ⟩ and |φ⟩, neither condition holds. Therefore, no such universal cloning operator exists.

## Significance
This fundamental quantum mechanical fact motivates why teleportation requires entanglement: you cannot copy an unknown state to measure it, so you must use pre-shared entanglement as a resource instead.

## Related Concepts
- [[Quantum Teleportation]]
- [[Measurement and State Collapse]]