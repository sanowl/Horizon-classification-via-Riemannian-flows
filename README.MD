# Horizon Riemannian Flows: A Mathematical Exploration

## 1. Introduction to Riemannian Flows on Horizons

Riemannian flows provide a powerful framework for understanding the geometry of horizons in general relativity. Let's break down the key components:

- **Manifold**: $$(H, g_T)$$ is a smooth $$(n+1)$$-dimensional manifold
- **Metric**: $$g_T$$ is a positive semi-definite symmetric bilinear form

A Riemannian flow on $$H$$ is characterized by:

1. A one-dimensional distribution $$D = \text{span}(n)$$, where $$n$$ is a non-vanishing vector field
2. Degeneracy condition: $$g_T(n, \cdot) = 0$$
3. Invariance property: $$\mathcal{L}_n g_T = 0$$ (Lie derivative along $$n$$)

In the context of general relativity:
- $$H$$ represents a horizon manifold
- $$n$$ is identified as the null generator of the horizon

### Key Theorem

For a null hypersurface $$H$$ in a Lorentzian manifold $$(M, g)$$:

The condition $$\mathcal{L}_n g_T = 0$$ is equivalent to $$H$$ being totally geodesic.

This theorem establishes the fundamental link between Riemannian flows and horizon geometry.

## 2. Geometric Structures on Horizons

### 2.1 Totally Geodesic Property

The totally geodesic nature of horizons is expressed by:

$$\nabla_X n = \omega(X)n, \quad \forall X \in \Gamma(TH)$$

Where:
- $$\nabla$$ is the Levi-Civita connection of the ambient spacetime restricted to $$H$$
- $$\omega \in \Omega^1(H)$$ is a one-form on $$H$$

### 2.2 Transverse Geometry

The quotient bundle $$Q = TH/D$$ inherits a rich geometric structure. The transverse Levi-Civita connection $$\nabla^T$$ on $$Q$$ satisfies:

1. $$\nabla^T_n \bar{X} = \overline{\mathcal{L}_n X}$$
2. $$\nabla^T g_T = 0$$
3. $$T^{\nabla^T}(\bar{X}, \bar{Y}) = 0$$ for all $$X, Y \in \Gamma(TH)$$

Here, the overline denotes projection onto $$Q$$.

## 3. Surface Gravity and Energy Conditions

Surface gravity $$\kappa$$ is defined as:

$$\kappa := \omega(n)$$

Under rescaling $$n' = e^f n$$, surface gravity transforms as:

$$\kappa' = e^f (\kappa + \partial_n f)$$

### Key Result

For a compact degenerate horizon $$H$$ in a spacetime satisfying the dominant energy condition:

$$\int_H \kappa\, d\tilde{g} = 0$$

Where:
- $$\tilde{g} = g_T + \alpha \otimes \alpha$$ is a Riemannian metric on $$H$$
- $$\alpha$$ is a 1-form such that $$\alpha(n) = 1$$

This provides a global constraint on surface gravity for degenerate horizons.

## 4. Classification of Compact Horizons

Compact horizons in 4-dimensional spacetimes can be classified as:

### a) Seifert Fibration
- All orbits are closed
- $$H$$ is a Seifert fibration over a Satake manifold
- Characterized by Seifert invariants $$(g, b; (\alpha_1, \beta_1), ..., (\alpha_k, \beta_k))$$

### b) Lens Space
- Two closed orbits, others densely fill 2-tori
- $$H$$ is diffeomorphic to a lens space $$L(p,q)$$ or $$S^1 \times S^2$$
- Flow on $$L(p,q)$$ represented as:
  $$\varphi_t: (z_1, z_2) \mapsto (e^{i\lambda t}z_1, e^{i\mu t}z_2)$$
  where $$\lambda/\mu$$ is irrational

### c) $$T^2$$ Bundle over $$S^1$$
- Every orbit densely fills a 2-torus
- $$H$$ is either diffeomorphic to $$T^3$$ or the hyperbolic fibration $$T^3_A$$
- For $$T^3_A$$:
  $$T^3_A = \mathbb{R} \times T^2 / \sim, \quad (x, v) \sim (x+1, A(v))$$
  where $$A \in SL(2, \mathbb{Z})$$ with $$\text{tr}(A) > 2$$

### d) Dense Flow on $$T^3$$
- All orbits are dense
- $$H$$ is diffeomorphic to $$T^3$$
- Flow given by:
  $$\dot{x} = a, \quad \dot{y} = b, \quad \dot{z} = c$$
  where $$a, b, c$$ are rationally independent

## 5. Analytical Tools for Riemannian Flows

Key analytical tools include:

1. **Basic Forms**: A k-form $$\omega$$ is basic if:
   $$i_n \omega = 0, \quad i_n d\omega = 0$$

2. **Mean Curvature Form**: Defined as:
   $$\mu := \mathcal{L}_n \chi$$
   where $$\chi$$ is the characteristic form of a bundle-like metric

3. **Molino's Structure Theorem**: For Riemannian flows with regular closure, the closures of the leaves form a singular Riemannian foliation, and the space of leaf closures has a natural Satake manifold structure.

These tools are crucial for analyzing the geometric and topological properties of horizons through Riemannian flow theory.