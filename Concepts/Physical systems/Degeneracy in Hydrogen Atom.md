The number of degenerate states (same energy) for each energy level in hydrogen.
## Quantum Number Constraints
For principal quantum number $n$:
- $l = 0, 1, 2, \ldots, n-1$ (n possible values)
- For each $l$: $m = -l, -l+1, \ldots, l$ (2l+1 values)
## Orbital Degeneracy
Total number of states with same $n$ (ignoring spin):
$$\sum_{l=0}^{n-1}(2l+1) = n^2$$

**Derivation**:
$$\sum_{l=0}^{n-1}(2l+1) = 2\sum_{l=0}^{n-1}l + \sum_{l=0}^{n-1}1 = 2\cdot\frac{(n-1)n}{2} + n = n^2$$
## Including Spin
Both electron and proton are spin-1/2 particles:
- 2 electron spin states
- 2 proton spin states
**Total degeneracy** = $4n^2$
For ground state ($n=1$): 4-fold degenerate
## Energy Levels
**$n=1$**: 1s → 4 states total
- $l=0$, $m=0$ with 4 spin combinations
**$n=2$**: 2s, 2p → 16 states total
- $l=0$ (2s): 1 state × 4 spins = 4 states
- $l=1$ (2p): 3 states × 4 spins = 12 states
**$n=3$**: 3s, 3p, 3d → 36 states total
- $l=0$ (3s): 4 states
- $l=1$ (3p): 12 states  
- $l=2$ (3d): 20 states
## Why m-Degeneracy?
**Expected**: Rotational symmetry means energy doesn't depend on orientation (m value).
External magnetic field would break this symmetry → Zeeman splitting.
## Why l-Degeneracy?
**Unexpected**: Called "accidental degeneracy" historically.
States with different $l$ (different effective potentials) have exactly the same energy! This is special to the $1/r$ Coulomb potential.
**Origin**: Hidden dynamical symmetry (Runge-Lenz vector conservation) specific to inverse-square force law.
## Lifting Degeneracy

**Fine structure** (Chapter 11): Relativistic effects split different $l$ states slightly ($\sim\alpha^2$ corrections)

**Hyperfine structure**: Spin interactions split states further

**External fields**: Electric or magnetic fields lift degeneracies

## Practical Importance

The $n^2$ degeneracy means many states have same energy. This affects:
- Statistical mechanics of hydrogen gas
- Selection rules for atomic transitions
- Structure of periodic table (Chapter 12)

Related: [[Energy Levels of Hydrogen Atom]], [[Hydrogen Wave Functions]], [[Complete Set of Commuting Observables]]
