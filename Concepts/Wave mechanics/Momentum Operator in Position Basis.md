## Representation in Position Space
In the position basis, the momentum operator is:
$$\hat{p}_x = -i\hbar\frac{\partial}{\partial x}$$

## Derivation from Translation
The infinitesimal translation operator:
$$\hat{T}(\delta x) = 1 - \frac{i}{\hbar}\hat{p}_x\delta x$$

Acting on a wave function:
$$\psi(x-\delta x) \approx \psi(x) - \delta x\frac{\partial\psi}{\partial x}$$

Comparing with T̂(δx)ψ(x) = [1 - (i/ℏ)p̂ₓδx]ψ(x):
$$\frac{i}{\hbar}\hat{p}_x\delta x\cdot\psi = \delta x\frac{\partial\psi}{\partial x}$$

Therefore:
$$\hat{p}_x = -i\hbar\frac{\partial}{\partial x}$$

## Acting on States
For any state |ψ⟩:
$$\langle x|\hat{p}_x|\psi\rangle = -i\hbar\frac{\partial}{\partial x}\langle x|\psi\rangle = -i\hbar\frac{\partial\psi(x)}{\partial x}$$

## Matrix Elements
$$\langle x|\hat{p}_x|x'\rangle = -i\hbar\frac{\partial}{\partial x}\delta(x-x')$$

## Physical Interpretation
- Derivatives measure rate of spatial variation
- Rapidly oscillating ψ(x) → high momentum
- Slowly varying ψ(x) → low momentum
- Pure plane wave e^(ipx/ℏ) has definite momentum p

## Connection to Classical Momentum
From Ehrenfest theorem:
$$\frac{d\langle x\rangle}{dt} = \frac{\langle \hat{p}_x\rangle}{m}$$

Average velocity equals average momentum divided by mass.