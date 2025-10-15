Three axes: a, b, c
In hidden variable model, each particle pair is type:

| Type | Particle 1 | Particle 2 |
|---|---|---|
| N₁ | {+a, +b, +c} | {-a, -b, -c} |
| N₂ | {+a, +b, -c} | {-a, -b, +c} |
| N₃ | {+a, -b, +c} | {-a, +b, -c} |
| N₄ | {+a, -b, -c} | {-a, +b, +c} |
| N₅ | {-a, +b, +c} | {+a, -b, -c} |
| N₆ | {-a, +b, -c} | {+a, -b, +c} |
| N₇ | {-a, -b, +c} | {+a, +b, -c} |
| N₈ | {-a, -b, -c} | {+a, +b, +c} |
## Define Three Sets
**Set AB:** Pairs where both give +ℏ/2 for measurements (a,b) = N₃ + N₄
**Set AC:** Pairs where both give +ℏ/2 for measurements (a,c) = N₂ + N₄
**Set CB:** Pairs where both give +ℏ/2 for measurements (c,b) = N₃ + N₇
Every pair in Set AB must appear in either Set AC or Set CB (or both).
#### The Inequality Holds
$$|AB| \leq |AC| + |CB|$$
In terms of populations:
$$N_3 + N_4 \leq (N_2 + N_4) + (N_3 + N_7)$$
## In Probabilities
Dividing by total number of pairs:
$$P(+a;+b) \leq P(+a;+c) + P(+c;+b)$$
**This must hold for any hidden variable theory.**
#### Quantum Mechanics Violates It
From [[Quantum Probability Derivation]]:
$$P(+a;+b) = \frac{1}{2}\sin^2\frac{\theta_{ab}}{2}$$
At θ_ab = 120°, θ_ac = 60°, θ_bc = 60°:
Left: (1/2)sin²(60°) = (1/2)·(3/4) = 3/8
Right: (1/2)sin²(30°) + (1/2)sin²(30°) = (1/2)·(1/4) + (1/2)·(1/4) = 1/4
**Result:** 3/8 > 1/4