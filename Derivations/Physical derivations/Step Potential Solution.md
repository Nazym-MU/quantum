# Step Potential Solution

## Problem Setup
Solve TISE for step potential:
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & x > 0 \end{cases}$$

Consider two cases: E > V₀ and E < V₀.

---

## Case 1: E > V₀

### Step 1: Write TISE in Each Region

**Region I (x < 0):**
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} = E\psi$$
$$\frac{d^2\psi}{dx^2} = -k^2\psi, \quad k = \frac{\sqrt{2mE}}{\hbar}$$

**Region II (x > 0):**
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V_0\psi = E\psi$$
$$\frac{d^2\psi}{dx^2} = -k_0^2\psi, \quad k_0 = \frac{\sqrt{2m(E-V_0)}}{\hbar}$$

### Step 2: General Solutions

**Region I:**
$$\psi_I(x) = Ae^{ikx} + Be^{-ikx}$$
- Ae^(ikx): incident wave (rightward)
- Be^(-ikx): reflected wave (leftward)

**Region II:**
$$\psi_{II}(x) = Ce^{ik_0x} + De^{-ik_0x}$$

**Physical boundary condition:** Set D = 0 (no source at x → +∞)
$$\psi_{II}(x) = Ce^{ik_0x}$$

### Step 3: Apply Boundary Conditions at x = 0

**Continuity of ψ:**
$$\psi_I(0) = \psi_{II}(0)$$
$$A + B = C \quad \text{...(1)}$$

**Continuity of ∂ψ/∂x:**
$$\frac{d\psi_I}{dx}\bigg|_{x=0} = \frac{d\psi_{II}}{dx}\bigg|_{x=0}$$
$$ik(A - B) = ik_0C \quad \text{...(2)}$$

### Step 4: Solve for Coefficients

From equation (2):
$$A - B = \frac{k_0}{k}C$$

Add equations (1) and modified (2):
$$2A = C\left(1 + \frac{k_0}{k}\right) = C\frac{k + k_0}{k}$$
$$C = \frac{2k}{k + k_0}A$$

Subtract to find B:
$$2B = C\left(1 - \frac{k_0}{k}\right) = C\frac{k - k_0}{k}$$

Substituting C:
$$B = \frac{k - k_0}{k + k_0}A$$

### Step 5: Calculate Reflection Coefficient

$$R = \frac{|B|^2}{|A|^2} = \left(\frac{k - k_0}{k + k_0}\right)^2$$

### Step 6: Calculate Transmission Coefficient

Using [[Probability Current]]:
$$j_{\text{inc}} = \frac{\hbar k}{m}|A|^2$$
$$j_{\text{trans}} = \frac{\hbar k_0}{m}|C|^2$$

$$T = \frac{j_{\text{trans}}}{j_{\text{inc}}} = \frac{k_0}{k}\frac{|C|^2}{|A|^2} = \frac{k_0}{k} \cdot \frac{4k^2}{(k+k_0)^2} = \frac{4kk_0}{(k+k_0)^2}$$

### Step 7: Verify Probability Conservation

$$R + T = \frac{(k-k_0)^2}{(k+k_0)^2} + \frac{4kk_0}{(k+k_0)^2}$$
$$= \frac{(k-k_0)^2 + 4kk_0}{(k+k_0)^2} = \frac{k^2 - 2kk_0 + k_0^2 + 4kk_0}{(k+k_0)^2}$$
$$= \frac{k^2 + 2kk_0 + k_0^2}{(k+k_0)^2} = \frac{(k+k_0)^2}{(k+k_0)^2} = 1 \quad \checkmark$$

---

## Case 2: E < V₀

### Step 1: Write TISE in Region II

**Region II (x > 0):**
$$\frac{d^2\psi}{dx^2} = \frac{2m(V_0 - E)}{\hbar^2}\psi = q^2\psi$$
where $$q = \frac{\sqrt{2m(V_0-E)}}{\hbar}$$

**General solution:**
$$\psi_{II}(x) = Fe^{qx} + Ge^{-qx}$$

**Physical boundary condition:** F = 0 (must decay as x → +∞)
$$\psi_{II}(x) = Ce^{-qx}$$

(Relabeled G → C for consistency)

### Step 2: Apply Boundary Conditions at x = 0

**Continuity of ψ:**
$$A + B = C \quad \text{...(1)}$$

**Continuity of ∂ψ/∂x:**
$$ik(A - B) = -qC \quad \text{...(2)}$$

### Step 3: Solve for Coefficients

From equations (1) and (2):
$$A - B = -\frac{q}{ik}C = \frac{iq}{k}C$$

Add:
$$2A = C\left(1 + \frac{iq}{k}\right) = C\frac{k + iq}{k}$$
$$C = \frac{2k}{k + iq}A$$

Subtract:
$$2B = C\left(1 - \frac{iq}{k}\right) = C\frac{k - iq}{k}$$
$$B = \frac{k - iq}{k + iq}A$$

### Step 4: Calculate Reflection Coefficient

$$|B|^2 = \left|\frac{k - iq}{k + iq}\right|^2 |A|^2 = \frac{|k - iq|^2}{|k + iq|^2}|A|^2 = \frac{k^2 + q^2}{k^2 + q^2}|A|^2 = |A|^2$$

Therefore:
$$R = \frac{|B|^2}{|A|^2} = 1$$

Total reflection!

### Step 5: Calculate Transmission Coefficient

For real exponential ψ = Ce^(-qx), the probability current is:
$$j_x = \frac{\hbar}{2mi}\left(\psi^*\frac{\partial\psi}{\partial x} - \psi\frac{\partial\psi^*}{\partial x}\right) = 0$$

(Since ψ is real: ψ* = ψ, so the two terms cancel exactly)

Therefore:
$$T = \frac{j_{\text{trans}}}{j_{\text{inc}}} = \frac{0}{j_{\text{inc}}} = 0$$

### Step 6: Verify R + T = 1

$$R + T = 1 + 0 = 1 \quad \checkmark$$

---

## Summary

| Case | R | T | Wave in Region II |
|------|---|---|-------------------|
| E > V₀ | (k-k₀)²/(k+k₀)² | 4kk₀/(k+k₀)² | Propagating (oscillatory) |
| E < V₀ | 1 | 0 | Evanescent (exponential decay) |

## Key Insight
Even when E > V₀, quantum mechanics predicts partial reflection (R ≠ 0). This is purely quantum effect with no classical analog.

## Related
- [[Potential Step Scattering]]
- [[Reflection Coefficient]]
- [[Transmission Coefficient]]
- [[Probability Current Derivation]]