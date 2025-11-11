The wave functions ψ(x) and ψ̃(p) are related by Fourier transforms. [[Fourier Identities]]
## Position → Momentum
$$\tilde{\psi}(p) = \langle p|\psi\rangle = \int_{-\infty}^{\infty} dx \, \langle p|x\rangle\langle x|\psi\rangle = \int_{-\infty}^{\infty} dx \, \frac{1}{\sqrt{2\pi\hbar}}e^{-ipx/\hbar}\psi(x)$$
## Momentum → Position
$$\psi(x) = \langle x|\psi\rangle = \int_{-\infty}^{\infty} dp \, \langle x|p\rangle\langle p|\psi\rangle = \int_{-\infty}^{\infty} dp \, \frac{1}{\sqrt{2\pi\hbar}}e^{ipx/\hbar}\tilde{\psi}(p)$$
To transform between bases, insert the identity:
**From x to p:** Insert Î = ∫dx |x⟩⟨x| between ⟨p| and |ψ⟩
**From p to x:** Insert Î = ∫dp |p⟩⟨p| between ⟨x| and |ψ⟩
## Dirac Delta Connection
The Fourier representation of the delta function:
$$\delta(x-x') = \frac{1}{2\pi\hbar}\int_{-\infty}^{\infty} e^{ip(x-x')/\hbar} dp$$

This is used to verify ⟨p'|p⟩ = δ(p'-p):
$$\langle p'|p\rangle = \int dx \, \langle p'|x\rangle\langle x|p\rangle$$
$$= \int dx \, \frac{1}{\sqrt{2\pi\hbar}}e^{-ip'x/\hbar} \cdot \frac{1}{\sqrt{2\pi\hbar}}e^{ipx/\hbar}$$
$$= \frac{1}{2\pi\hbar}\int dx \, e^{i(p-p')x/\hbar} = \delta(p-p')$$

## Physical Meaning
- Localized in position ↔ spread out in momentum
- Localized in momentum ↔ spread out in position
- Cannot be sharp in both (uncertainty principle)

## Example: Gaussian
A Gaussian in position space:
$$\psi(x) = \frac{1}{(\pi a^2)^{1/4}}e^{-x^2/(2a^2)}$$

Fourier transforms to Gaussian in momentum space:
$$\tilde{\psi}(p) = \frac{a^{1/2}}{(\pi\hbar^2)^{1/4}}e^{-p^2a^2/(2\hbar^2)}$$