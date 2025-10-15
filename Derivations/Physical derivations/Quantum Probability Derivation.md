Derivation: P(+a;+b) = (1/2)sin²(θ_ab/2)
## Setup
Two particles in singlet state:
$$|0,0\rangle = \frac{1}{\sqrt{2}}|+z,-z\rangle - \frac{1}{\sqrt{2}}|-z,+z\rangle$$
Alice measures particle 1 along **a** → gets +ℏ/2. Particle 2 collapses to |-a⟩.
Bob measures particle 2 along **b**. What's probability he gets +ℏ/2?

From [[Spin Overlap Derivation]], we know:
$$\langle +b|+a\rangle = \cos\frac{\theta_{ab}}{2}$$
If angle between a and b is $θ_ab$, then angle between -a and b is $π - θ_ab$.
$$\langle +b|-a\rangle = \cos\frac{\pi - \theta_{ab}}{2} = \cos\left(\frac{\pi}{2} - \frac{\theta_{ab}}{2}\right) = \sin\frac{\theta_{ab}}{2}$$

Same sign probability: $\sin^2\frac{\theta_{ab}}{2}$
By symmetry of singlet state: equal numbers of (++) and (--) pairs. So probability of (++) is half of "same sign":
$$\boxed{P(+a;+b) = \frac{1}{2}\sin^2\frac{\theta_{ab}}{2}}$$
- θ_ab = 0: P = 0 ✓ (if particle 1 is +a, particle 2 is -a)
- θ_ab = 90°: P = (1/2)·(1/√2)² = 1/4
- θ_ab = 180°: P = (1/2)·1² = 1/2 ✓