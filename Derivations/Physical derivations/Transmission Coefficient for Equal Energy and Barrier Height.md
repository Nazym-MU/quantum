# Transmission Coefficient for Equal Energy and Barrier Height

## Problem
Calculate transmission coefficient when particle energy equals barrier height: E = V₀.

## Setup
Square barrier:
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & 0 < x < a \\ 0 & x > a \end{cases}$$

with E = V₀.

---

## Step 1: Wave Functions

**Region I (x < 0):**
$$\psi_I(x) = Ae^{ikx} + Be^{-ikx}$$
where $$k = \frac{\sqrt{2mE}}{\hbar} = \frac{\sqrt{2mV_0}}{\hbar}$$

**Region II (0 < x < a):**
At E = V₀, the kinetic energy in region II is zero:
$$\frac{d^2\psi}{dx^2} = 0$$

General solution is **linear**:
$$\psi_{II}(x) = C + Dx$$

**Region III (x > a):**
$$\psi_{III}(x) = Fe^{ikx}$$

---

## Step 2: Boundary Conditions at x = 0

**Continuity of ψ:**
$$A + B = C \quad \text{...(1)}$$

**Continuity of ∂ψ/∂x:**
$$ik(A - B) = D \quad \text{...(2)}$$

From (2): $$D = ik(A - B)$$

---

## Step 3: Boundary Conditions at x = a

**Continuity of ψ:**
$$C + Da = Fe^{ika} \quad \text{...(3)}$$

**Continuity of ∂ψ/∂x:**
$$D = ikFe^{ika} \quad \text{...(4)}$$

---

## Step 4: Solve for Coefficients

From equation (4):
$$F = \frac{D}{ik}e^{-ika}$$

Substitute into equation (3):
$$C + Da = \frac{D}{ik}e^{-ika} \cdot e^{ika} = \frac{D}{ik}$$
$$C = \frac{D}{ik} - Da = D\left(\frac{1}{ik} - a\right)$$

From equation (2): D = ik(A - B)

Substitute:
$$C = ik(A - B)\left(\frac{1}{ik} - a\right) = (A - B)(1 - ika)$$

From equation (1): C = A + B

Equate:
$$A + B = (A - B)(1 - ika)$$
$$A + B = A - B - ikaA + ikaB$$
$$2B = -ikaA + ikaB - A$$
$$2B - ikaB = -A(1 + ika)$$
$$B(2 - ika) = -A(1 + ika)$$

From equations (1) and (2):
$$2A = C + \frac{D}{ik} = C - ia \cdot D/k$$

We also have C = A + B and D = ik(A - B):
$$2A = (A + B) - ia \cdot i(A - B) = A + B + a(A - B)$$
$$2A = A(1 + a) + B(1 - a)$$
$$A(1 - a) = B(1 - a)$$

**Correction:** Let me redo this systematically.

From (2): A - B = D/(ik)
From (1): A + B = C

Add: 2A = C + D/(ik)
From (3): C = Fe^(ika) - Da
From (4): D = ikFe^(ika)

Substitute (4) into (3):
$$C = Fe^{ika} - ikFe^{ika} \cdot a = Fe^{ika}(1 - ika)$$

So: 2A = Fe^(ika)(1 - ika) + Fe^(ika)
$$2A = Fe^{ika}(2 - ika)$$
$$F = \frac{2e^{-ika}}{2 - ika}A$$

---

## Step 5: Calculate Transmission Coefficient

$$T = \frac{|F|^2}{|A|^2} = \frac{4}{|2 - ika|^2} = \frac{4}{4 + k^2a^2}$$

$$T = \frac{1}{1 + (ka/2)^2}$$

---

## Step 6: Limiting Behavior

**As a → 0 (barrier vanishes):**
$$T \to 1$$
Complete transmission.

**As a → ∞ (thick barrier):**
$$T \to 0$$
Transmission vanishes.

**For ka = 2 (resonance condition):**
$$T = \frac{1}{1 + 1} = \frac{1}{2}$$

---

## Physical Interpretation

Even at E = V₀ (threshold energy), a finite barrier causes partial reflection. The wave in region II is constant slope (zero curvature) rather than oscillatory or exponential.

This is the limiting case between:
- E > V₀: oscillatory in barrier
- E < V₀: exponential decay in barrier

---

## Related
- [[Transmission Coefficient]]
- [[Potential Barrier Scattering]]
- [[Step Potential Solution]]