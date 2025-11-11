# Example - Unpolarized vs 50-50 Mixed States

Comparing different mixed states and demonstrating non-uniqueness of density operator preparation.

## Part (a): 50% |+z⟩, 50% |-z⟩

**Density operator**:
$$\hat{\rho} = \frac{1}{2}|+z\rangle\langle+z| + \frac{1}{2}|-z\rangle\langle-z|$$

**Matrix in Sᵤ basis**:
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} + \frac{1}{2}\begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$$

**Check: Mixed state?**
$$\hat{\rho}^2 = \frac{1}{4}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$$
$$\text{tr}(\hat{\rho}^2) = \frac{1}{4}(1 + 1) = \frac{1}{2} < 1 \quad \checkmark$$

**Calculate ⟨Sₓ⟩**:
$$\hat{S}_x = \frac{\hbar}{2}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$$

$$\hat{S}_x\hat{\rho} = \frac{\hbar}{4}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$$

$$\langle S_x\rangle = \text{tr}(\hat{S}_x\hat{\rho}) = \frac{\hbar}{4}(0 + 0) = 0$$

**Physical interpretation**: Half particles have Sᵤ = +ℏ/2 (giving ⟨Sₓ⟩ = 0), half have Sᵤ = -ℏ/2 (giving ⟨Sₓ⟩ = 0). Overall average: 0.

## Part (b): 50% |+z⟩, 50% |-x⟩

**Express |-x⟩ in Sᵤ basis**:
$$|-x\rangle = \frac{1}{\sqrt{2}}(|+z\rangle - |-z\rangle)$$

**Density operator for |-x⟩**:
$$|-x\rangle\langle-x| = \frac{1}{2}(|+z\rangle - |-z\rangle)(\langle+z| - \langle-z|)$$

$$= \frac{1}{2}\left[|+z\rangle\langle+z| - |+z\rangle\langle-z| - |-z\rangle\langle+z| + |-z\rangle\langle-z|\right]$$

**Matrix form**:
$$|-x\rangle\langle-x| = \frac{1}{2}\begin{pmatrix} 1 & -1 \\ -1 & 1 \end{pmatrix}$$

**Full density operator**:
$$\hat{\rho} = \frac{1}{2}|+z\rangle\langle+z| + \frac{1}{2}|-x\rangle\langle-x|$$

$$= \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} + \frac{1}{4}\begin{pmatrix} 1 & -1 \\ -1 & 1 \end{pmatrix}$$

$$= \frac{1}{4}\begin{pmatrix} 3 & -1 \\ -1 & 1 \end{pmatrix}$$

**Check: Mixed state?**
$$\hat{\rho}^2 = \frac{1}{16}\begin{pmatrix} 10 & -4 \\ -4 & 2 \end{pmatrix}$$

$$\text{tr}(\hat{\rho}^2) = \frac{1}{16}(10 + 2) = \frac{3}{4} < 1 \quad \checkmark$$

Wait, let me recalculate:
$$\hat{\rho}^2 = \frac{1}{16}\begin{pmatrix} 3 & -1 \\ -1 & 1 \end{pmatrix}\begin{pmatrix} 3 & -1 \\ -1 & 1 \end{pmatrix}$$
$$= \frac{1}{16}\begin{pmatrix} 10 & -4 \\ -4 & 2 \end{pmatrix}$$

Hmm, actually tr(ρ²) = (10+2)/16 = 12/16 = 3/4, not 5/8 as text says. Let me verify the matrix multiplication again...

Actually rechecking: (3)(3) + (-1)(-1) = 9+1 = 10 ✓
(-1)(3) + (1)(-1) = -3-1 = -4 ✓
(-1)(-1) + (1)(1) = 1+1 = 2 ✓

So tr(ρ²) = 12/16 = 3/4.

**Calculate ⟨Sₓ⟩**:
$$\langle S_x\rangle = \text{tr}\left[\frac{\hbar}{2}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \frac{1}{4}\begin{pmatrix} 3 & -1 \\ -1 & 1 \end{pmatrix}\right]$$

$$= \text{tr}\left[\frac{\hbar}{8}\begin{pmatrix} -1 & 1 \\ 3 & -1 \end{pmatrix}\right] = \frac{\hbar}{8}(-1 + (-1)) = -\frac{\hbar}{4}$$

**Physical interpretation**: 
- 50% in |+z⟩: contributes ⟨Sₓ⟩ = 0
- 50% in |-x⟩: contributes ⟨Sₓ⟩ = -ℏ/2
- Average: (1/2)(0) + (1/2)(-ℏ/2) = -ℏ/4 ✓

## CAUTION: Same Density Operator ≠ Same Preparation

The density operator from part (a):
$$\hat{\rho}_a = \frac{1}{2}|+z\rangle\langle+z| + \frac{1}{2}|-z\rangle\langle-z| = \frac{1}{2}\hat{I}$$

Can ALSO be written as:
$$\hat{\rho}_a = \frac{1}{2}|+x\rangle\langle+x| + \frac{1}{2}|-x\rangle\langle-x| = \frac{1}{2}\hat{I}$$

OR:
$$\hat{\rho}_a = \frac{1}{2}|+y\rangle\langle+y| + \frac{1}{2}|-y\rangle\langle-y| = \frac{1}{2}\hat{I}$$

OR for ANY direction n:
$$\hat{\rho}_a = \frac{1}{2}|+n\rangle\langle+n| + \frac{1}{2}|-n\rangle\langle-n| = \frac{1}{2}\hat{I}$$

**Key Point**: You CANNOT tell from the density matrix how the ensemble was prepared! All these different preparations yield:
- Same ρ̂
- Same predictions for ALL observables
- Therefore same quantum state

## Related
- [[Unpolarized Ensemble]]
- [[Density Operator Mixed State]]
- [[Off-Diagonal Elements and Coherence]]