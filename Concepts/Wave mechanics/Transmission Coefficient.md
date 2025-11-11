# Transmission Coefficient

## Definition
The probability that a particle incident on a potential is transmitted through rather than reflected.

## Mathematical Definition
$$T = \frac{j_{\text{trans}}}{j_{\text{inc}}}$$

where:
- j_inc: incident [[Probability Current]]
- j_trans: transmitted probability current (must use actual current, not just amplitude)

## Probability Conservation
Must satisfy: R + T = 1, where R is the [[Reflection Coefficient]].

## Examples

### Potential Step (E > V₀)
$$T = \frac{4kk_0}{(k + k_0)^2}$$
where k = √(2mE)/ℏ and k₀ = √(2m(E-V₀))/ℏ.

Note: Even though E > V₀, transmission is not perfect (T < 1) due to quantum reflection.

### Potential Step (E < V₀)
$$T = 0$$
No transmission through infinite step when E < V₀, even though wave penetrates (evanescent).

### Potential Barrier (E < V₀, finite width a)
$$T = \frac{1}{1 + \frac{(k^2 + q^2)^2}{4k^2q^2}\sinh^2(qa)}$$

where q = √(2m(V₀-E))/ℏ.

For wide barriers (qa >> 1):
$$T \approx \frac{16k^2q^2}{(k^2+q^2)^2}e^{-2qa}$$

### E = V₀ Case
Special case where k₀ = 0 for step or barrier:
$$T = \frac{1}{1 + (ka/2)^2}$$
See [[Transmission Coefficient for Equal Energy and Barrier Height]].

## Critical Distinction
T is NOT simply |C|²/|A|² in general. Must account for velocity difference:
$$T = \frac{v_{\text{trans}}}{v_{\text{inc}}} \frac{|C|^2}{|A|^2} = \frac{k_0}{k}\frac{|C|^2}{|A|^2}$$

This is why T = 0 for E < V₀ step even though C ≠ 0: the velocity (and current) in the barrier is zero.

## Physical Interpretation
T is the fraction of incident particles transmitted through the potential. For [[Quantum Tunneling]], this represents tunneling probability.

## Related
- [[Reflection Coefficient]]
- [[Potential Step Scattering]]
- [[Potential Barrier Scattering]]
- [[Quantum Tunneling]]