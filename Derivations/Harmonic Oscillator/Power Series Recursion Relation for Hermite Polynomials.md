## Starting Point
From [[Differential Equation for h(y)]]:
$$\frac{d^2h}{dy^2} - 2y\frac{dh}{dy} + (\varepsilon - 1)h = 0$$
## Power Series Ansatz
Assume solution has form:
$$h(y) = \sum_{k=0}^{\infty} a_k y^k = a_0 + a_1 y + a_2 y^2 + a_3 y^3 + \cdots$$
This is valid for analytic functions (like polynomials and many special functions).
## Computing Derivatives
First derivative:
$$\frac{dh}{dy} = \sum_{k=0}^{\infty} ka_k y^{k-1} = \sum_{k=1}^{\infty} ka_k y^{k-1}$$
(k=0 term vanishes)
Second derivative:
$$\frac{d^2h}{dy^2} = \sum_{k=1}^{\infty} k(k-1)a_k y^{k-2} = \sum_{k=2}^{\infty} k(k-1)a_k y^{k-2}$$
(k=0,1 terms vanish)
## Substituting into Differential Equation
$$\sum_{k=2}^{\infty} k(k-1)a_k y^{k-2} - 2y\sum_{k=1}^{\infty} ka_k y^{k-1} + (\varepsilon-1)\sum_{k=0}^{\infty} a_k y^k = 0$$
Simplify middle term:
$$\sum_{k=2}^{\infty} k(k-1)a_k y^{k-2} - 2\sum_{k=1}^{\infty} ka_k y^k + (\varepsilon-1)\sum_{k=0}^{\infty} a_k y^k = 0$$
## Index Shifting
**Problem**: First sum has y^(k-2), others have y^k. Need same power in all sums.
**Solution**: In first sum, substitute k' = k - 2, so k = k' + 2:
- When k = 2, k' = 0
- When k → ∞, k' → ∞

$$\sum_{k=2}^{\infty} k(k-1)a_k y^{k-2} = \sum_{k'=0}^{\infty} (k'+2)(k'+1)a_{k'+2} y^{k'}$$

**Rename** k' → k (dummy variable):
$$= \sum_{k=0}^{\infty} (k+2)(k+1)a_{k+2} y^k$$

## Combining All Terms

Now all sums have y^k:
$$\sum_{k=0}^{\infty} (k+2)(k+1)a_{k+2} y^k - 2\sum_{k=1}^{\infty} ka_k y^k + (\varepsilon-1)\sum_{k=0}^{\infty} a_k y^k = 0$$

Note: Second sum starts at k=1 (k=0 term vanishes anyway since it's 2·0·a₀ = 0), so we can write all from k=0:
$$\sum_{k=0}^{\infty} \left[(k+2)(k+1)a_{k+2} - 2ka_k + (\varepsilon-1)a_k\right] y^k = 0$$

## Linear Independence of Powers
Since {1, y, y², y³, ...} are linearly independent, the only way this sum equals zero for all y is if each coefficient vanishes:
$$(k+2)(k+1)a_{k+2} - 2ka_k + (\varepsilon-1)a_k = 0$$
## Recursion Relation
Solve for a_(k+2):
$$(k+2)(k+1)a_{k+2} = [2k - (\varepsilon-1)]a_k = (2k + 1 - \varepsilon)a_k$$
$$a_{k+2} = \frac{2k + 1 - \varepsilon}{(k+2)(k+1)} a_k$$
## Consequences
**Even/odd separation**:
- Given a₀, the recursion determines a₂, a₄, a₆, ... (even series)
- Given a₁, the recursion determines a₃, a₅, a₇, ... (odd series)
- These are independent
**Solution structure**:
h(y) = (even polynomial) + (odd polynomial)
For unique solutions, typically set either a₀ or a₁ to zero.
## Related
- Previous: [[Differential Equation for h(y)]]
- Next: [[Series Termination and Energy Quantization]]
- Used in: [[Week 11.2 - Position Space Solution and Parity]]