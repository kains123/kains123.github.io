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

**Divergence Operator in Phase Space** is

The divergence operator $$\(\nabla\_{\mathbf{Z}}\)$$ in phase space is defined as:

\[
\nabla*{\mathbf{Z}} = \left(\frac{\partial}{\partial q_1}, \ldots, \frac{\partial}{\partial q*{3N}}, \frac{\partial}{\partial p*1}, \ldots, \frac{\partial}{\partial p*{3N}}\right).
\]

This operator takes into account all position and momentum coordinates in the \(6N\)-dimensional space.

### 5. **Applying the Divergence Theorem**

To derive the continuity equation in phase space, we use the **divergence theorem**, which states:

\[
\int*{\Omega} \nabla*{\mathbf{Z}} \cdot (\rho \dot{\mathbf{Z}}) \, d\mathbf{Z} = \int\_{S} (\rho \dot{\mathbf{Z}}) \cdot d\mathbf{S},
\]

where:

- \(\Omega\) is an arbitrary volume in phase space.
- \(S\) is the boundary surface of \(\Omega\).

The left side represents the total divergence of the probability current inside \(\Omega\), and the right side represents the flux of this current across the boundary \(S\). For any arbitrary choice of \(\Omega\), the equality implies the local form of the continuity equation:

\[
\frac{\partial \rho}{\partial t} + \nabla\_{\mathbf{Z}} \cdot (\rho \dot{\mathbf{Z}}) = 0.
\]

### 6. **ensemble density**

We can expand the divergence term \(\nabla\_{\mathbf{Z}} \cdot (\rho \dot{\mathbf{Z}})\):

\[
\nabla*{\mathbf{Z}} \cdot (\rho \dot{\mathbf{Z}}) = \dot{\mathbf{Z}} \cdot \nabla*{\mathbf{Z}} \rho + \rho \nabla\_{\mathbf{Z}} \cdot \dot{\mathbf{Z}},
\]

where:

- \(\dot{\mathbf{Z}} \cdot \nabla\_{\mathbf{Z}} \rho\) represents the **advection** of the ensemble density along the flow in phase space.
- \(\rho \nabla\_{\mathbf{Z}} \cdot \dot{\mathbf{Z}}\) represents the **divergence of the phase space velocity**.

### 7. **Material Derivative and Liouville's Equation**

We can introduce the **material derivative** (or total derivative) to describe the change in \(\rho\) as we move with the flow in phase space:

\[
\frac{D\rho}{Dt} \equiv \frac{\partial \rho}{\partial t} + \dot{\mathbf{Z}} \cdot \nabla\_{\mathbf{Z}} \rho.
\]

The continuity equation can now be rewritten using the material derivative:

\[
\frac{D\rho}{Dt} = -\rho \nabla\_{\mathbf{Z}} \cdot \dot{\mathbf{Z}}.
\]

In a **conservative system**, where the phase space flow is incompressible (\(\nabla\_{\mathbf{Z}} \cdot \dot{\mathbf{Z}} = 0\)), this simplifies to:

\[
\frac{D\rho}{Dt} = 0 \implies \frac{\partial \rho}{\partial t} + \dot{\mathbf{Z}} \cdot \nabla\_{\mathbf{Z}} \rho = 0.
\]

This is known as **Liouville's equation**, which states that the ensemble density is constant along the trajectories of the system in phase space.

### 8. **Conclusion**

- The **continuity equation in phase space** mirrors the mass continuity equation in fluid dynamics, expressing the conservation of probability density rather than mass.
- The velocity \(\dot{\mathbf{Z}}\) in phase space is analogous to the fluid velocity \(\mathbf{u}\).
- **Liouville's theorem** implies that, for a conservative system, the density of microstates in phase space remains constant as the system evolves.

This analogy provides a powerful way to understand the behavior of complex systems in statistical mechanics using concepts familiar from fluid dynamics.
