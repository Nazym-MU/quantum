# Plane Wave Direction of Travel

## Time-Dependent Wave Function

A stationary state with definite energy E has time dependence:
$$\Psi(x,t) = \psi(x)e^{-iEt/\hbar}$$

Using E = ℏω:
$$\Psi(x,t) = \psi(x)e^{-i\omega t}$$

---

## Rightward Traveling Wave

For spatial part ψ(x) = e^(ikx):
$$\Psi(x,t) = e^{i(kx - \omega t)}$$

**Constant phase condition:**
$$kx - \omega t = \text{constant}$$

Differentiate with respect to time:
$$k\frac{dx}{dt} - \omega = 0$$
$$\frac{dx}{dt} = \frac{\omega}{k} > 0$$

Wave travels in **+x direction** (rightward).

---

## Leftward Traveling Wave

For spatial part ψ(x) = e^(-ikx):
$$\Psi(x,t) = e^{-i(kx + \omega t)}$$

**Constant phase condition:**
$$kx + \omega t = \text{constant}$$

Differentiate:
$$k\frac{dx}{dt} + \omega = 0$$
$$\frac{dx}{dt} = -\frac{\omega}{k} < 0$$

Wave travels in **-x direction** (leftward).

---

## Physical Interpretation

The sign in the spatial exponential determines propagation direction:
- **Positive** exponent e^(+ikx): rightward
- **Negative** exponent e^(-ikx): leftward

This is why scattering solutions use:
$$\psi(x) = Ae^{ikx} + Be^{-ikx}$$
- A term: incident/transmitted wave (→)
- B term: reflected wave (←)

---

## Probability Current Direction

For ψ = Ae^(ikx):
$$j_x = \frac{\hbar k}{m}|A|^2 > 0$$
Positive current (rightward flow).

For ψ = Be^(-ikx):
$$j_x = -\frac{\hbar k}{m}|B|^2 < 0$$
Negative current (leftward flow).

The [[Probability Current]] direction matches the wave propagation direction.

---

## Related
- [[Momentum Eigenstates]] - e^(ikx) is eigenstate of momentum operator with eigenvalue ℏk
- [[Probability Current]]
- [[Potential Step Scattering]]
- [[Unbound States]]