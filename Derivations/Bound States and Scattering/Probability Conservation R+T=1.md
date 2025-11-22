# Probability Conservation: R + T = 1

## Statement
For any scattering process, the [[Reflection Coefficient]] and [[Transmission Coefficient]] must satisfy:
$$R + T = 1$$

This follows from [[Probability Current]] conservation.

## Setup

Consider steady-state scattering (time-independent states). Divide space into three regions:
- **Left region (x < 0):** incident + reflected waves
- **Scattering region:** potential present
- **Right region (x > x₀):** transmitted wave only

## Step 1: Wave Functions

**Left region:**
$$\psi_L(x) = Ae^{ikx} + Be^{-ikx}$$

**Right region:**
$$\psi_R(x) = Ce^{ik'x}$$

where k and k' may differ if potential changes energy.

## Step 2: Probability Currents

From [[Probability Current Derivation]]:
$$j = \frac{\hbar k}{m}(|A|^2 - |B|^2)$$

**Incident current:**
$$j_{inc} = \frac{\hbar k}{m}|A|^2$$

**Reflected current (magnitude):**
$$|j_{ref}| = \frac{\hbar k}{m}|B|^2$$

**Transmitted current:**
$$j_{trans} = \frac{\hbar k'}{m}|C|^2$$

## Step 3: Continuity Equation

For time-independent states:
$$\frac{\partial \rho}{\partial t} = 0$$

where ρ = |ψ|² is probability density.

From continuity equation:
$$\frac{\partial \rho}{\partial t} + \frac{\partial j}{\partial x} = 0$$

Therefore:
$$\frac{\partial j}{\partial x} = 0$$

Current is constant in space (no accumulation).

## Step 4: Current Balance

Net current entering from left = net current exiting to right:
$$j_{inc} - |j_{ref}| = j_{trans}$$

$$\frac{\hbar k}{m}|A|^2 - \frac{\hbar k}{m}|B|^2 = \frac{\hbar k'}{m}|C|^2$$

Divide by j_inc = (ℏk/m)|A|²:
$$1 - \frac{|B|^2}{|A|^2} = \frac{k'}{k}\frac{|C|^2}{|A|^2}$$

## Step 5: Identify R and T

**Reflection coefficient:**
$$R = \frac{|j_{ref}|}{j_{inc}} = \frac{|B|^2}{|A|^2}$$

**Transmission coefficient:**
$$T = \frac{j_{trans}}{j_{inc}} = \frac{k'}{k}\frac{|C|^2}{|A|^2}$$

Note: The k'/k factor accounts for velocity change!

## Step 6: Conservation Law

Substituting into the current balance equation:
$$1 - R = T$$

Therefore:
$$R + T = 1$$

## Physical Interpretation

- Every incident particle is either reflected or transmitted
- No particle is created or destroyed
- Probability is conserved globally
- Current continuity ensures local conservation

## Special Cases

**Same potential asymptotically (k' = k):**
$$T = \frac{|C|^2}{|A|^2}$$

**Step with E < V₀:**
- j_trans = 0 (no actual flow in barrier)
- R = 1, T = 0

**Barrier with E < V₀:**
- Nonzero transmission through barrier
- R < 1, T > 0

## Related
- [[Probability Current Derivation]]
- [[Reflection Coefficient]]
- [[Transmission Coefficient]]
- [[Step Potential Solution]]
- [[Barrier Tunneling Solution]]