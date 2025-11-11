## Goal
Show that [x̂, p̂ₓ] = iℏ from the translation operator properties.

## Setup
The translation operator satisfies:
$$\hat{T}(\delta x) = 1 - \frac{i}{\hbar}\hat{p}_x\delta x$$
$$\hat{T}(\delta x)|x\rangle = |x + \delta x\rangle$$

## Step 1: Commutator with Position
Consider the commutator [x̂, T̂(δx)]:
$$[\hat{x}, \hat{T}(\delta x)] = \hat{x}\hat{T}(\delta x) - \hat{T}(\delta x)\hat{x}$$

## Step 2: Act on Position Eigenstate
Apply both sides to |x⟩:
$$\hat{x}\hat{T}(\delta x)|x\rangle = \hat{x}|x+\delta x\rangle = (x+\delta x)|x+\delta x\rangle$$

$$\hat{T}(\delta x)\hat{x}|x\rangle = \hat{T}(\delta x)(x|x\rangle) = x|x+\delta x\rangle$$

## Step 3: Compute Difference
$$[\hat{x}, \hat{T}(\delta x)]|x\rangle = (x+\delta x)|x+\delta x\rangle - x|x+\delta x\rangle = \delta x|x+\delta x\rangle$$

For small δx: |x+δx⟩ ≈ |x⟩, so:
$$[\hat{x}, \hat{T}(\delta x)] = \delta x$$

## Step 4: Substitute Generator Form
$$[\hat{x}, 1 - \frac{i}{\hbar}\hat{p}_x\delta x] = \delta x$$

Since [x̂, Î] = 0:
$$-\frac{i}{\hbar}[\hat{x}, \hat{p}_x]\delta x = \delta x$$

## Result
$$[\hat{x}, \hat{p}_x] = i\hbar$$

This fundamental commutator is the origin of the uncertainty principle and distinguishes quantum from classical mechanics.