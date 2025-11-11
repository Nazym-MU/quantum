Derives general uncertainty relation for any observable Â:
$$\Delta A \cdot \Delta t ≥ \frac{\hbar}{2}$$
where $$\Delta t = \frac{\Delta A}{|d⟨A⟩/dt|}$$
## Step 1: Time Derivative of Expectation Value
For time-independent operator Â:
$$\frac{d⟨A⟩}{dt} = \frac{d}{dt}⟨ψ|Â|ψ⟩$$
Using Schrödinger equation iℏ∂|ψ⟩/∂t = Ĥ|ψ⟩:
$$\frac{d⟨A⟩}{dt} = \frac{1}{iℏ}⟨ψ|[Ĥ, Â]|ψ⟩ = \frac{i}{ℏ}⟨[Â, Ĥ]⟩$$
## Step 2: Apply General Uncertainty Relation
From \[Â, Ĥ\] = iĈ where Ĉ = iℏ(d⟨A⟩/dt):
$$\Delta A \cdot \Delta E ≥ \frac{|\langle C \rangle|}{2} = \frac{\hbar}{2}\left|\frac{d⟨A⟩}{dt}\right|$$
## Step 3: Define Δt
Rearrange:
$$\Delta E ≥ \frac{\hbar}{2\Delta A}\left|\frac{d⟨A⟩}{dt}\right|$$
Define characteristic timescale:
$$\Delta t = \frac{\Delta A}{|d⟨A⟩/dt|}$$
This is the time for ⟨A⟩ to change by amount ~ΔA.
## Step 4: Final Result
$$\boxed{\Delta E \cdot \Delta t ≥ \frac{\hbar}{2}}$$
## Physical Meaning
Δt is **not** uncertainty in time. It's the evolutionary timescale - how long to wait before measurements of A show noticeable change.
## See
- [[Energy-Time Uncertainty Relation]]
- [[Uncertainty Relations Schwarz Inequality Derivation]]