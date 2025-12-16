# Positronium Ionization Energy

Calculation of ionization energy for positronium (electron-positron bound state).

## What is Positronium?

Bound state of electron ($e^-$) and positron ($e^+$) - the antiparticle of electron.

Like hydrogen, but:
- "Nucleus" is positron instead of proton
- Both particles have equal mass

## Energy Formula

For hydrogenic atom:
$$E_n = -\frac{\mu c^2 Z^2 \alpha^2}{2n^2}$$

For positronium: $Z = 1$ (positron has charge $+e$)

## Reduced Mass

For hydrogen: $\mu_H = \frac{m_e m_p}{m_e + m_p} \approx m_e\left(1 - \frac{m_e}{m_p}\right) \approx 0.9995 m_e$

For positronium: $m_1 = m_2 = m_e$

$$\mu_{\text{Ps}} = \frac{m_e \cdot m_e}{m_e + m_e} = \frac{m_e^2}{2m_e} = \frac{m_e}{2}$$

## Energy Levels of Positronium

$$E_n^{\text{Ps}} = -\frac{(\mu_{\text{Ps}}) c^2 \alpha^2}{2n^2} = -\frac{(m_e/2) c^2 \alpha^2}{2n^2}$$

$$= -\frac{m_e c^2 \alpha^2}{4n^2} = -\frac{13.6 \text{ eV}}{2n^2}$$

## Ground State Energy

$$E_1^{\text{Ps}} = -\frac{13.6 \text{ eV}}{2} = -6.8 \text{ eV}$$

## Ionization Energy

Energy needed to ionize (separate electron and positron to infinity with zero kinetic energy):

$$E_{\text{ionization}} = |E_1^{\text{Ps}}| = \boxed{6.8 \text{ eV}}$$

This is exactly **half** the ionization energy of hydrogen (13.6 eV).

## Physical Reason

The factor of 1/2 comes entirely from the reduced mass being half that of hydrogen:

$$\frac{E_1^{\text{Ps}}}{E_1^{\text{H}}} = \frac{\mu_{\text{Ps}}}{\mu_H} \approx \frac{m_e/2}{m_e} = \frac{1}{2}$$

## Lifetime

Positronium is **unstable** - electron and positron annihilate into photons.

Can only annihilate in $l=0$ states (need spatial overlap).

**Ground state** ($l=0$):
- Singlet (antiparallel spins): lifetime ~125 ps → 2 photons
- Triplet (parallel spins): lifetime ~142 ns → 3 photons

**Excited states** ($l > 0$): Must first decay to ground state before annihilation.

## Why This Example Matters

Demonstrates that:
1. Quantum mechanics applies to exotic systems (matter-antimatter)
2. Reduced mass corrections are measurable
3. Only $l=0$ states allow annihilation (spatial overlap requirement)

Related: [[Energy Levels of Hydrogen Atom]], [[Reduced Mass]], [[Radial Wave Function Near Origin]]
