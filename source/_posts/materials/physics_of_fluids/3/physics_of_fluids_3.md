---
title: 3. From Statistical Mechanics to Thermodynamics
date:
  "[object Object]": null
categories:
  - materials
  - physics of fluids
mathjax: true
---

### 3.1 Liouville's the theorem and equation

The total number of ensemble members is constant. So phase space volume $$\Omega$$ must be equal to the rate at which the ensemble members leave $$\Omega$$ through the surface S.

This is exactly same conditon that we impose to derive the mass continuity equation.

ex) Phase Space Equation

\begin{eqnarray\*}
\nabla\cdot\vec{E}&=&\frac{\rho}{\epsilon_0}\\\\
\nabla\cdot\vec{B}&=&0\\\\
\nabla\times\vec{E}&=&-\frac{\partial B}{\partial t}\\\\
\nabla\times\vec{B}&=&\mu_0\left(\vec{J}+\epsilon_0\frac{\partial E}{\partial t}\right)\\\\
\end{eqnarray\*}

$$
\int_{\Omega} \frac{\partial \rho}{\partial t} \, \mathrm{d}Z = - \oint_{S} \rho \, (\dot{Z} \cdot \hat{n}) \, \mathrm{d}S
$$

ex) Fluid Dynamics Equation

$$
\int_{V} \frac{\partial \rho}{\partial t} \, \mathrm{d}V = - \oint_{S} \rho \, (\mathbf{u} \cdot \hat{n}) \, \mathrm{d}S
$$

In statistical mechanics, we consider the phase space, which is a 6𝑁 dimensional space for a system with 𝑁 particles. Each point in this space is represented by:

$$
\[
\mathbf{Z} = (q_1, q_2, \ldots, q_{3N}, p_1, p_2, \ldots, p_{3N}).
\]
$$

where:
$$q_i$$ are the position coordinates.
$$p_i$$ are the momentum coordinates.

We can imagine $$ \dot{Z} $$ as "velocity" in the phase space.

$$\(\rho(\mathbf{Z}, t)\)$$ be the **ensemble density** in phase space
So the **continuity equation in phase space** is ..

$$
\[
\frac{\partial \rho}{\partial t} + \nabla\_{\mathbf{Z}} \cdot (\rho \dot{\mathbf{Z}}) = 0.
\]
$$

$$
\[
\frac{\partial \rho}{\partial t} + \nabla\_{\mathbf{Z}} \cdot (\rho \dot{\mathbf{Z}}) = 0,
\]
$$

where:

- $$\(\nabla\_{\mathbf{Z}}\)$$ is the divergence operator in the $$\(6N\)$$-dimensional phase space.
- $$\(\rho \dot{\mathbf{Z}}\)$$ represents the **probability current** in phase space.

**1. Liouville equation**
Hamiltonian dynamics can be described as an incompressible flow in phase space.

$$\frac{D\Omega}{Dt} = \frac{\partial \Omega}{\partial t} + \dot{Z} \cdot \nabla_Z \Omega = 0$$

**2. Liouville Operator and Poisson Brackets**

- Liouville equation II
  $$\frac{\partial \Omega}{\partial t} = -i\mathcal{L} \Omega$$

$\mathcal{L}$ is the Liouville operator, which can be defined using Possion brackets.

$$
i\mathcal{L}\rho = \dot{Z} \cdot \nabla_Z \rho,
$$

- Poisson bracket
  $$
  \{A, B\} = \sum_{\alpha=1}^{3N} \left( \frac{\partial A}{\partial q_\alpha} \frac{\partial B}{\partial p_\alpha} - \frac{\partial A}{\partial p_\alpha} \frac{\partial B}{\partial q_\alpha} \right).
  $$

Thus, Liouville Equation is

$$
\frac{\partial \rho}{\partial t} = -\{ \rho, H \}
$$

If the phase space distribution function \(\rho(Z, t)\) is conserved, it implies:

$$
\{ \rho, H \} = 0.
$$

- Phase Space Volume Preservation

$$
\int \rho(Z, 0) \, dZ_0 = \int \rho(Z, t) \, dZ_t
$$

## 3.2 Statistical Ensembles in Equilibrium

1. Equilibrium Condition
   For a system to be in equilibrium, the phase space distribution function $\(\rho(Z, t)\)$ should not explicitly depend on time:

   $frac{\partial \rho}{\partial t} = 0$
   $\{\rho, H\} = 0$$\

2. **Ergodic Hypothesis**
   The ergodic hypothesis states that, given an infinite amount of time, an ergodic system will eventually visit all possible states that are accessible to it.

   For **Hamiltonian systems**, this implies that the system will cover all points on a hypersurface where the Hamiltonian \( H \) is constant.

**Ensemble and Temporal Average**
In an ergodic system, the **ensemble average** of a quantity $A$ is equivalent to its **temporal average**
$$A = \langle a \rangle = \lim_{T \to \infty} \frac{1}{T} \int_0^T a(Z(t)) \, dt$$

3. types of statistical ensembles

   The types of statistical ensembles are classified based on the quantities held constant:
   ex) **Microcanonical Ensemble** ($\(N, V, E = \text{const.}\)$):

   - Represents an **isolated** system with fixed particle number \(N\), volume \(V\), and energy \(E\).
   - The system follows Hamiltonian dynamics, and the total energy is conserved.

   **Canonical Ensemble** ($\(N, V, T = \text{const.}\)$):

   - Represents a system in contact with a **heat bath** at a fixed temperature $T$.
   - The total energy of the system is not conserved because it can exchange energy with the heat bath.

## 3.3 Basic Thermodynamics

**Definitions**
A thermodynamics system is a macroscopic system. The thermodynamic state of the system is uniquely defined by specification of a set of control variables, e.g, temperature, pressure, volume etc.

Two types of thermodynamic variables:

- extensive variables are proportional to the system size (ex. internal energy, mass, entropy)
- intensive variables are independent of the system size (ex. pressure, temperature, density, chemial potential)

$pV = nRT$

## 3.4 Laws of Thermodynamics

- Zeroth Law (0법칙)
  Establishes the concept of temperature and thermal equilibrium. If two systems are in thermal equilibrium with a third system, they are also in equilibrium with each other.

- First Law (1법칙)
  The conservation energy. The energy E of the system can be changed by performing work W on it and/or by adding heat Q to it
  $dE = \delta W + \delta Q$

- Second Law (2법칙)
  $dS \geq \frac{\delta Q}{T}$

- Third Law
  The entropy of a system at the absolute zero temperature is a universal constant, which we can set to zero. The T = 0K temperature can never be physically reached.
