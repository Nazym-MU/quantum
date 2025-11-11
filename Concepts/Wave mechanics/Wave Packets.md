A wave packet is a superposition of momentum eigenstates:
$$|\psi\rangle = \int dp \, |p\rangle\langle p|\psi\rangle = \int dp \, |p\rangle\tilde{\psi}(p)$$

## Physical Motivation
**Problem:** Pure momentum eigenstates |p⟩ are not physical:
- Δp = 0 but Δx = ∞
- Cannot normalize: ∫|⟨x|p⟩|²dx = ∞

**Solution:** Superpose many momentum states to create localized packets:
- 0 < Δp < ∞ (finite momentum spread)
- 0 < Δx < ∞ (finite position spread)
- ΔxΔp ≥ ℏ/2 (uncertainty principle satisfied)

## Classical Analogy
Like a clap of thunder:
- Contains many frequencies (momentum states)
- Localized in time/space (wave packet)
- Not a pure tone (not a pure momentum state)

## General Properties
**In position space:**
$$\psi(x) = \int dp \, \frac{1}{\sqrt{2\pi\hbar}}e^{ipx/\hbar}\tilde{\psi}(p)$$

Constructive interference where phases align → localization.

**In momentum space:**
$$\tilde{\psi}(p) = \int dx \, \frac{1}{\sqrt{2\pi\hbar}}e^{-ipx/\hbar}\psi(x)$$

Spread in p-space determines localization in x-space.

## Key Insight
Wave packets are the physical states that:
- Can be prepared experimentally
- Have finite uncertainties in both x and p
- Evolve in time according to Schrödinger equation
- Reduce to classical particles in appropriate limits

## Connection to Uncertainty
The width of ψ̃(p) determines Δp.
The width of ψ(x) determines Δx.
These are inversely related: narrow in one → broad in the other.