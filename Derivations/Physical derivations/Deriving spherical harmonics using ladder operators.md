1. Start with highest $m$ state: $|l, l\rangle$
2. Use condition $\hat{L}_+|l, l\rangle = 0$
3. Apply lowering operator repeatedly to generate $|l, m\rangle$ for all $m$
## Step 1: Condition for Highest State
$$\hat{L}_+|l, l\rangle = 0$$
In position space with $\hat{L}_+ = -i\hbar e^{i\phi}\left(\frac{\partial}{\partial\theta} + i\cot\theta\frac{\partial}{\partial\phi}\right)$:
$$e^{i\phi}\left(\frac{\partial}{\partial\theta} + i\cot\theta\frac{\partial}{\partial\phi}\right)\langle\theta, \phi|l, l\rangle = 0$$
## Step 2: Insert Known φ Dependence
We know $\langle\theta, \phi|l, l\rangle = f(\theta)e^{il\phi}$ from $\hat{L}_z$ eigenvalue equation.
Substituting:
$$e^{i\phi}\left(\frac{df}{d\theta} + i\cot\theta(il)f\right)e^{il\phi} = 0$$
$$\frac{df}{d\theta} - l\cot\theta \, f = 0$$
## Step 3: Solve Differential Equation
$$\frac{df}{f} = l\cot\theta \, d\theta = l \frac{d(\sin\theta)}{\sin\theta}$$
$$\ln f = l\ln(\sin\theta) + C$$
$$f(\theta) = A\sin^l\theta$$
## Step 4: Normalization
Using $\int_0^\pi \sin\theta \, d\theta \int_0^{2\pi} d\phi \, |Y_{l,l}|^2 = 1$:
$$Y_{l,l}(\theta, \phi) = (-1)^l\sqrt{\frac{(2l+1)!}{4\pi \cdot 2^l l!}} e^{il\phi}\sin^l\theta$$
Phase factor $(-1)^l$ is conventional.
## Step 5: Generate Other States
Use lowering operator relation:
$$\hat{L}_-|l, m\rangle = \sqrt{l(l+1) - m(m-1)}\hbar|l, m-1\rangle$$
In position space:
$$Y_{l,m-1} = \frac{1}{\sqrt{l(l+1) - m(m-1)}\hbar}\hat{L}_- Y_{l,m}$$
## General Formula Result
For $m \geq 0$:
$$Y_{l,m}(\theta, \phi) = (-1)^l\sqrt{\frac{2l+1}{4\pi}\frac{(l+m)!}{(l-m)!}} e^{im\phi}\frac{1}{\sin^m\theta}\frac{d^{l-m}}{d(\cos\theta)^{l-m}}\sin^{2l}\theta$$
For $m < 0$:
$$Y_{l,m} = (-1)^m Y_{l,-m}^*$$
Related: [[Explicit Spherical Harmonic Functions]], [[Spherical Harmonics Definition]]
