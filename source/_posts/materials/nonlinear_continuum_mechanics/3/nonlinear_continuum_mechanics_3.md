---
title: 3. Kinematics
date:
  "[object Object]": null
categories:
  - materials
  - nonlinear continuum mechanics
mathjax: true
---

### 3.1 Configuration and motion spatial

A spatial domain $\Omega_0$ and is supposed to be stress free. The reference configuration is $t = 0$. The current configuration at time $t$.

$T = [0, t_{\text{end}}]$ denotes the time interval of interest. Note that a fixed

$\mathbf{\underline{X}}$ for all times points to a specific material element. Therefore $\mathbf{\underline{X}}$ can directly be identified with material elements. Furthermore, assuming that the deformation map is invertible.

$\mathbf{\underline{X}} = \mathbf{f}^{-1}(\mathbf{\underline{x}}, t)$

Lagrangian description: mechnaical physics -> reference configuration, material coordinates.
Eulerian description: fluid mechanics -> current configuration, spatial coordinates.

### 3.2 Displacement, velocity and acceleration

A mathmatical description for the motion of a continuum (Lagangian):
$$\underline{U}(\underline{X}, t) = \underline{x}(\underline{X}, t) - \underline{X}$$

A spatial coodinates for the motion of a continuum (Eulerian):
$$\underline{u}(\underline{x}, t) = \underline{x} - \underline{X}(\underline{x}, t)$$
