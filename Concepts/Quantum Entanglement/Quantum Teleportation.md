## Definition
Quantum teleportation is the transfer of an unknown quantum state from one location (Alice) to another (Bob) using an entangled pair and classical communication. The original state is destroyed in the process.

## The Problem It Solves
Cannot determine an arbitrary quantum state |ψ⟩ = a|+z⟩ + b|−z⟩ by measurement alone—measurement collapses the state and we lose the relative phase between amplitudes. The [[No-Cloning Theorem]] proves we cannot copy an unknown state to measure it repeatedly. Therefore, direct "scanning" of the state is impossible.

## The Protocol

**Setup:**
- Particle 1: unknown state |ψ₁⟩ (Alice's particle)
- Particles 2 & 3: entangled in [[Singlet State]] |0,0⟩₂₃ (EPR pair)
- Particle 2 goes to Alice, particle 3 goes to Bob

**Steps:**
1. Alice performs a [[Bell State Measurement]] on particles 1 and 2 (projects onto Bell basis)
2. Alice gets one of four results, each with probability 1/4
3. Alice sends the 2-bit classical result to Bob
4. Bob applies a unitary rotation to particle 3 based on Alice's result
5. Particle 3 is now in state |ψ⟩

**Key fact:** The three-particle state before Alice's measurement is |ψ₁⟩ ⊗ |0,0⟩₂₃. Particles 1 and 2 are initially *not entangled*, only 2 and 3 are. Alice's measurement creates entanglement between 1 and 2 while transferring the state information to 3.

## Why It's Not Faster-Than-Light Communication
Bob's particle after Alice's measurement is a random mixture of four possible states—it gives no information about |ψ⟩ until he receives Alice's classical message. If Bob guesses before the message arrives, he recovers only noise.

## Why It Works
Entanglement allows correlated measurement outcomes without local realism. When Alice measures particles 1 and 2, particle 3's state is instantaneously determined (up to a known unitary). The classical channel tells Bob which unitary to apply.

## Related Concepts
- [[No-Cloning Theorem]]
- [[Singlet State]]
- [[Bell State Measurement]]
- [[EPR Pair]]
- [[Local Realism]]