## Problem Setup
Solve TISE for square barrier with E < V₀:
$$V(x) = \begin{cases} 0 & x < 0 \\ V_0 & 0 < x < a \\ 0 & x > a \end{cases}$$

Particle incident from left with energy E < V₀ (classically forbidden).
---

## Step 1: Write Wave Functions in Each Region

**Region I (x < 0):**
$$\psi_I(x) = Ae^{ikx} + Be^{-ikx}$$
where $$k = \frac{\sqrt{2mE}}{\hbar}$$

**Region II (0 < x < a):**
$$\psi_{II}(x) = Fe^{qx} + Ge^{-qx}$$
where $$q = \frac{\sqrt{2m(V_0-E)}}{\hbar}$$

Both exponentials needed (finite width barrier).

**Region III (x > a):**
$$\psi_{III}(x) = Ce^{ikx}$$
No incident wave from right (D = 0).

---

## Step 2: Apply Boundary Conditions at x = 0

**Continuity of ψ:**
$$\psi_I(0) = \psi_{II}(0)$$
$$A + B = F + G \quad \text{...(1)}$$

**Continuity of ∂ψ/∂x:**
$$\frac{d\psi_I}{dx}\bigg|_{x=0} = \frac{d\psi_{II}}{dx}\bigg|_{x=0}$$
$$ik(A - B) = q(F - G) \quad \text{...(2)}$$

---

## Step 3: Apply Boundary Conditions at x = a

**Continuity of ψ:**
$$\psi_{II}(a) = \psi_{III}(a)$$
$$Fe^{qa} + Ge^{-qa} = Ce^{ika} \quad \text{...(3)}$$

**Continuity of ∂ψ/∂x:**
$$\frac{d\psi_{II}}{dx}\bigg|_{x=a} = \frac{d\psi_{III}}{dx}\bigg|_{x=a}$$
$$q(Fe^{qa} - Ge^{-qa}) = ikCe^{ika} \quad \text{...(4)}$$

---

## Step 4: Eliminate F and G

From equations (3) and (4):

**From (3):**
$$Fe^{qa} + Ge^{-qa} = Ce^{ika} \quad \text{...(3)}$$

**From (4):**
$$Fe^{qa} - Ge^{-qa} = \frac{ik}{q}Ce^{ika} \quad \text{...(4')}$$

**Add (3) and (4'):**
$$2Fe^{qa} = Ce^{ika}\left(1 + \frac{ik}{q}\right)$$
$$F = \frac{1}{2}\left(1 + \frac{ik}{q}\right)Ce^{i ka - qa} \quad \text{...(5)}$$

**Subtract (4') from (3):**
$$2Ge^{-qa} = Ce^{ika}\left(1 - \frac{ik}{q}\right)$$
$$G = \frac{1}{2}\left(1 - \frac{ik}{q}\right)Ce^{ika + qa} \quad \text{...(6)}$$

---

## Step 5: Eliminate B

From equations (1) and (2):

**From (1):**
$$A + B = F + G$$

**From (2):**
$$A - B = \frac{q}{ik}(F - G) = -i\frac{q}{k}(F - G)$$

**Add:**
$$2A = (F + G) - i\frac{q}{k}(F - G)$$
$$2A = F\left(1 - i\frac{q}{k}\right) + G\left(1 + i\frac{q}{k}\right)$$

Substitute F and G from equations (5) and (6):
$$2A = \frac{Ce^{ika}}{2}\left[\left(1 + \frac{ik}{q}\right)e^{-qa}\left(1 - i\frac{q}{k}\right) + \left(1 - \frac{ik}{q}\right)e^{qa}\left(1 + i\frac{q}{k}\right)\right]$$

**Expand first term:**
$$\left(1 + \frac{ik}{q}\right)\left(1 - i\frac{q}{k}\right) = 1 - i\frac{q}{k} + \frac{ik}{q} + \frac{q}{k} \cdot \frac{k}{q} = 1 - i\frac{q}{k} + \frac{ik}{q} + 1$$
$$= 2 + i\left(\frac{k}{q} - \frac{q}{k}\right)$$

**Expand second term:**
$$\left(1 - \frac{ik}{q}\right)\left(1 + i\frac{q}{k}\right) = 1 + i\frac{q}{k} - \frac{ik}{q} + \frac{q}{k} \cdot \frac{k}{q} = 1 + i\frac{q}{k} - \frac{ik}{q} + 1$$
$$= 2 - i\left(\frac{k}{q} - \frac{q}{k}\right)$$

**Combine:**
$$2A = \frac{Ce^{ika}}{2}\left[e^{-qa}\left(2 + i\left(\frac{k}{q} - \frac{q}{k}\right)\right) + e^{qa}\left(2 - i\left(\frac{k}{q} - \frac{q}{k}\right)\right)\right]$$

$$= Ce^{ika}\left[e^{-qa} + e^{qa} + i\left(\frac{k}{q} - \frac{q}{k}\right)\frac{e^{-qa} - e^{qa}}{2}\right]$$

$$= Ce^{ika}\left[2\cosh(qa) - i\left(\frac{k}{q} - \frac{q}{k}\right)\sinh(qa)\right]$$

$$= Ce^{ika}\left[2\cosh(qa) - i\frac{k^2 - q^2}{kq}\sinh(qa)\right]$$

---

## Step 6: Calculate Transmission Coefficient

$$T = \frac{j_{\text{trans}}}{j_{\text{inc}}} = \frac{|C|^2}{|A|^2}$$

(Since k same in regions I and III)

From Step 5:
$$\frac{C}{A} = \frac{2e^{-ika}}{2\cosh(qa) - i\frac{k^2 - q^2}{kq}\sinh(qa)}$$

$$\left|\frac{C}{A}\right|^2 = \frac{4}{4\cosh^2(qa) + \left(\frac{k^2-q^2}{kq}\right)^2\sinh^2(qa)}$$

Using cosh²(qa) - sinh²(qa) = 1:
$$\cosh^2(qa) = 1 + \sinh^2(qa)$$

$$\left|\frac{C}{A}\right|^2 = \frac{4}{4(1 + \sinh^2(qa)) + \frac{(k^2-q^2)^2}{k^2q^2}\sinh^2(qa)}$$

$$= \frac{4}{4 + \left[4 + \frac{(k^2-q^2)^2}{k^2q^2}\right]\sinh^2(qa)}$$

$$= \frac{4}{4 + \frac{4k^2q^2 + (k^2-q^2)^2}{k^2q^2}\sinh^2(qa)}$$

Expand numerator: 4k²q² + k⁴ - 2k²q² + q⁴ = k⁴ + 2k²q² + q⁴ = (k² + q²)²

$$T = \frac{1}{1 + \frac{(k^2+q^2)^2}{4k^2q^2}\sinh^2(qa)}$$

---

## Step 7: Wide Barrier Approximation (qa >> 1)

For qa >> 1:
$$\sinh(qa) = \frac{e^{qa} - e^{-qa}}{2} \approx \frac{e^{qa}}{2}$$

$$\sinh^2(qa) \approx \frac{e^{2qa}}{4}$$

$$T \approx \frac{1}{\frac{(k^2+q^2)^2}{16k^2q^2}e^{2qa}} = \frac{16k^2q^2}{(k^2+q^2)^2}e^{-2qa}$$

Dominant behavior: **exponential suppression** ∝ e^(-2qa).

---

## Physical Interpretation

1. **Tunneling occurs:** T ≠ 0 even though E < V₀
2. **Exponential suppression:** Thicker/higher barriers → smaller T
3. **Reflection not total:** R = 1 - T < 1
4. **Microscopic phenomenon:** For typical atomic parameters, T can be O(1)
5. **Macroscopic suppression:** For macroscopic parameters, T ~ e^(-10^27) ≈ 0

---

## Summary

**Exact transmission coefficient:**
$$T = \frac{1}{1 + \frac{(k^2+q^2)^2}{4k^2q^2}\sinh^2(qa)}$$

**Wide barrier limit:**
$$T \approx \frac{16k^2q^2}{(k^2+q^2)^2}e^{-2qa}$$

**Reflection coefficient:**
$$R = 1 - T$$

## Related
- [[Potential Barrier Scattering]]
- [[Quantum Tunneling]]
- [[Transmission Coefficient]]
- [[Step Potential Solution]]