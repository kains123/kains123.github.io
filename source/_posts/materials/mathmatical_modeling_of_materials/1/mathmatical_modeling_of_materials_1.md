---
title: 2. Mathematical preliminaries
date:
  "[object Object]": null
categories:
  - materials
  - nonlinear continuum mechanics
mathjax: true
---

### 2.1 Conventions

T : arbitrary-order tensor.

### 2.2 Definition of a tensor

We can construct tensors of arbitary order n by concatenating n bases using the tensor product . For instance, a second-order tensor results from:

$$
\underline{\underline{\mathbf{T}}} = T\_{ij}\underline{\mathbf{g}}\_i \otimes \underline{\mathbf{g}}\_j
$$

### 2.3. Tensor calculus

Let’s go over the **cross product** definition, the role of the **Levi-Civita symbol**, and how they are used together to express the cross product of two vectors.

#### 2.3.1. **Cross Product Definition**

The cross product $$\mathbf{u} \times \mathbf{v}$$

- Is **perpendicular (two lines, planes, or vectors that meet at a right angle (90 degrees))** to both $$\mathbf{u}$$ and $$\mathbf{v}.$$

The cross product in terms of vector components is given by:

$$
\mathbf{u} \times \mathbf{v} = (u_y v_z - u_z v_y, \, u_z v_x - u_x v_z, \, u_x v_y - u_y v_x).
$$

**Levi-Civita Symbol $$\(\epsilon\_{ijk}\)$$**

The **Levi-Civita symbol** $$\(\epsilon\_{ijk}\)$$ is used to simplify expressions involving cross products in three dimensions.

$$[\mathbf{u} \times \mathbf{v}]_i = \epsilon_{ijk} u_j v_k$$

#### 2.3.5 Tensor analysis

**1. Gradient of a Tensor Field**
The gradient of a function is the collection of its partial derivatives. When we apply the gradient operator $$\nabla$$ to a tensor field, the order of the resulting tensor increases by one.

$$
   [ \text{grad}\, u ]_{ij} = [ \nabla u ]_{ij} = \frac{\partial u_i}{\partial x_j} = u_{i,j}.
$$

**1.1 Partial Derivative**

$$
\frac{\partial (\cdot)}{\partial x*i} = (\cdot)*{,i}.
$$

**2. Divergence Operator**

The **divergence** of a vector or tensor field is defined. The divergence measures the "spread" or "flux" of a vector field.

**Divergence of a Vector Field**

$$\text{div}\, u = \nabla \cdot u = \frac{\partial u*i}{\partial x_i} = u*{i,i}.$$
