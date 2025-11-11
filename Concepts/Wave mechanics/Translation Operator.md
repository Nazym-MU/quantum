The translation operator $\hat T(a)$ shifts position states:
$$\hat{T}(a)|x\rangle = |x+a\rangle$$
## Action on General States
For any state |ψ⟩:
$$|\psi'\rangle = \hat{T}(a)|\psi\rangle$$
$$\psi'(x) = \langle x|\psi'\rangle = \psi(x-a)$$
**Physical meaning:** State shifts right by a → wave function argument shifts left by a.
## Key Properties
**Unitary:**
- Preserves normalization: ⟨ψ'|ψ'⟩ = ⟨ψ|ψ⟩
- Invertible: $\hat T^{-1}(a) = \hat{T}(-a)=\hat{T}^\dagger (a)$
**Group property:**
$$\hat{T}(a)\hat{T}(b) = \hat{T}(a+b)$$
## Generator Form
**Infinitesimal translation:**
$$\hat{T}(\delta x) = 1 - \frac{i}{\hbar}\hat{p}_x \delta x$$
**Finite translation:**
$$\hat{T}(a) = e^{-i\hat{p}_x a/\hbar}$$
The momentum operator $p̂_x$ generates translations in space.