![[SG experiment 5 drawing.png]]

> Complex numbers are essential to describe the transformations.

Mathematical description (formulas - [[<3>]]):
$$\bra{+y} = \frac{e^{-i\gamma_+}}{\sqrt{2}}\bra{+z} + \frac{e^{-i\gamma_-}}{\sqrt{2}}\bra{-z} = \frac{e^{-i\gamma_+}}{\sqrt{2}}\left[ \bra{+z}+r^{-i(\gamma_- - \gamma_+)}\bra{-z} \right] \text{ and } \gamma = \gamma_--\gamma_+$$

$$\ket{+x} = \frac{e^{i\beta_+}}{\sqrt{2}}\ket{+z} + \frac{e^{i\beta_-}}{\sqrt{2}}\ket{-z} = \frac{e^{-i\beta_+}}{\sqrt{2}}\left[ \ket{+z}+r^{-i(\beta_- - \beta_+)}\ket{-z} \right]  \text{ and } \beta = \beta_--\beta_+$$
Find the probability of |+x⟩ from SGx device ending up in the state |+y⟩:
$$\braket{+y|+z} = \frac{e^{i(\beta_+-\gamma_+)}}{2}\cdot \left[ 1 + e^{i(\beta - \gamma)}\right]$$
β and γ are [[Relative phases]] between the kets
Probability [[(5)]]: 
$$|\braket{+y|+z}|^2 = \frac{1}{4}\left[ 1 + e^{i(\beta - \gamma)}\right]\cdot \left[ 1 + e^{-i(\beta - \gamma)}\right] = \frac{1}{2}\left[ 1 + \cos(\beta - \gamma)\right] = \frac{1}{2}$$ Therefore, β - γ has to be ±π/2