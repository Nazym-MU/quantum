# Example - Computing Expectation Values with Density Operator

Computing ⟨Sᵧ⟩ for pure states using density operator formalism.

## Part (a): State |+z⟩

**Density operator in Sᵤ basis**:
$$\hat{\rho} = |+z\rangle\langle+z| = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$$

**Sᵧ operator in Sᵤ basis**:
$$\hat{S}_y = \frac{\hbar}{2}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}$$

**Matrix product**:
$$\hat{S}_y\hat{\rho} = \frac{\hbar}{2}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} = \frac{\hbar}{2}\begin{pmatrix} 0 & 0 \\ i & 0 \end{pmatrix}$$

**Trace (sum diagonal elements)**:
$$\langle S_y\rangle = \text{tr}(\hat{S}_y\hat{\rho}) = \frac{\hbar}{2}(0 + 0) = 0$$

**Physical interpretation**: Measuring Sᵧ on |+z⟩ gives ±ℏ/2 with equal probability (50% each), so average is zero.

## Part (b): State |+y⟩

**Express in Sᵤ basis**:
$$|+y\rangle = \frac{1}{\sqrt{2}}(|+z\rangle + i|-z\rangle)$$

**Density operator**:
$$\hat{\rho} = |+y\rangle\langle+y| = \frac{1}{2}(|+z\rangle + i|-z\rangle)(\langle+z| - i\langle-z|)$$

**Expand the outer product**:
$$= \frac{1}{2}\left[|+z\rangle\langle+z| - i|+z\rangle\langle-z| + i|-z\rangle\langle+z| + |-z\rangle\langle-z|\right]$$

**Matrix form in Sᵤ basis**:
$$\hat{\rho} = \frac{1}{2}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$

Note: Off-diagonal elements (-i and i) encode the relative phase!

**Matrix product**:
$$\hat{S}_y\hat{\rho} = \frac{\hbar}{2}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} \frac{1}{2}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$

$$= \frac{\hbar}{4}\begin{pmatrix} 0 \cdot 1 + (-i) \cdot i & 0 \cdot (-i) + (-i) \cdot 1 \\ i \cdot 1 + 0 \cdot i & i \cdot (-i) + 0 \cdot 1 \end{pmatrix}$$

$$= \frac{\hbar}{4}\begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}$$

**Trace**:
$$\langle S_y\rangle = \text{tr}(\hat{S}_y\hat{\rho}) = \frac{\hbar}{4}(1 + 1) = \frac{\hbar}{2}$$

**Physical interpretation**: |+y⟩ is eigenstate of Ŝᵧ with eigenvalue ℏ/2, so ⟨Sᵧ⟩ = ℏ/2 with 100% certainty.

## Key Insight
The relative phase between basis states shows up in off-diagonal matrix elements of the density operator. This phase information is essential for calculating expectation values correctly.

## Related
- [[Expectation Values from Density Operator]]
- [[Off-Diagonal Elements and Coherence]]
- [[Spin Operators (Pauli Matrices)]]