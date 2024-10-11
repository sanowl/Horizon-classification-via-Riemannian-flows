
# Detailed Explanation of Horizon Riemannian Flows

## 1. Riemannian Flows

A Riemannian flow is a special case of a Riemannian foliation where the leaves are one-dimensional. Let $$(H, g_T)$$ be a smooth manifold with a positive semi-definite symmetric bilinear form $$g_T$$. The Riemannian flow structure is defined by:

1. A one-dimensional distribution $$D = \text{span}(n)$$, where $$n$$ is a non-vanishing vector field.
2. $$g_T(n, \cdot) = 0$$
3. $$\mathcal{L}_n g_T = 0$$, where $$\mathcal{L}_n$$ denotes the Lie derivative along $$n$$.

In the context of horizons, $$H$$ represents the horizon manifold, and $$n$$ is the null generator of the horizon.

## 2. Totally Geodesic Property

For a horizon $$H$$, the totally geodesic property is expressed as:

$$\nabla_X n = \omega(X)n$$

where $$X$$ is an arbitrary vector field tangent to $$H$$, $$\nabla$$ is the Levi-Civita connection, and $$\omega$$ is a one-form on $$H$$.

## 3. Surface Gravity

The surface gravity $$\kappa$$ is defined as:

$$\kappa := \omega(n)$$

Under a rescaling $$n' = e^f n$$, the surface gravity transforms as:

$$\kappa' = e^f (\kappa + \partial_n f)$$

## 4. Classification Theorem (Theorem 2.23)

The classification of compact horizons in 4-dimensional spacetimes yields the following possibilities:

a) **Seifert Fibration**: All orbits are closed. $$H$$ is a Seifert fibration over a Satake manifold.

b) **Lens Space**: Two closed orbits, others densely fill 2-tori. $$H$$ is diffeomorphic to a lens space $$L(p,q)$$ or $$S^1 \times S^2$$.

c) **$$T^2$$ Bundle over $$S^1$$**: Every orbit densely fills a 2-torus. $$H$$ is a $$T^2$$-bundle over $$S^1$$, either diffeomorphic to $$T^3$$ or the hyperbolic fibration $$T^3_A$$.

d) **Dense Flow on $$T^3$$**: All orbits are dense. $$H$$ is diffeomorphic to $$T^3$$.

## 5. Mathematical Details of Each Case

### 5.1 Seifert Fibration

A Seifert fibration is a generalization of a circle bundle. For a base space $$B$$ and fiber $$S^1$$, the total space $$H$$ is locally of the form $$D^2 \times S^1$$ with the gluing map:

$$(r, \theta, \phi) \mapsto (r, \theta, p\phi + q\theta)$$

where $$p$$ and $$q$$ are coprime integers. The Seifert invariants $$(g, b; (\alpha_1, \beta_1), ..., (\alpha_k, \beta_k))$$ characterize the fibration, where $$g$$ is the genus of the base orbifold, $$b$$ is the Euler number of the bundle, and $$(\alpha_i, \beta_i)$$ represent the exceptional fibers.

### 5.2 Lens Space

A lens space $$L(p,q)$$ is obtained by gluing two solid tori along their boundaries. The gluing map is given by:

$$f: S^1 \times S^1 \to S^1 \times S^1, \quad f(\theta, \phi) = (p\theta + q\phi, -r\theta + s\phi)$$

where $$ps - qr = 1$$. The flow on $$L(p,q)$$ can be represented as:

$$\varphi_t: (z_1, z_2) \mapsto (e^{i\lambda t}z_1, e^{i\mu t}z_2)$$

where $$\lambda/\mu$$ is irrational.

### 5.3 $$T^2$$ Bundle over $$S^1$$

For the case of a $$T^2$$ bundle over $$S^1$$, we have two subcases:

a) $$T^3$$: The flow can be represented by a linear flow on the 3-torus:

$$\dot{x} = a, \quad \dot{y} = b, \quad \dot{z} = c$$

where $$a, b, c$$ are rationally independent.

b) Hyperbolic $$T^3_A$$: This is a suspension of a hyperbolic automorphism of $$T^2$$. The flow is given by:

$$T^3_A = \mathbb{R} \times T^2 / \sim, \quad (x, v) \sim (x+1, A(v))$$

where $$A \in SL(2, \mathbb{Z})$$ with $$\text{tr}(A) > 2$$.

### 5.4 Dense Flow on $$T^3$$

For a dense flow on $$T^3$$, we have a linear flow:

$$\dot{x} = a, \quad \dot{y} = b, \quad \dot{z} = c$$

where $$a, b, c$$ are rationally independent, ensuring that every orbit is dense in $$T^3$$.

## 6. Riemannian Flow Structure Analysis

The Riemannian flow structure can be analyzed using the following tools:

1. **Transverse Levi-Civita Connection**: Defined by:

   $$\nabla^T_X \bar{Y} = \overline{\nabla_X Y}$$

   where $$\bar{Y}$$ is the projection of $$Y$$ onto the quotient bundle $$Q = TH/L$$.

2. **Basic Forms**: A k-form $$\omega$$ is basic if:

   $$i_n \omega = 0, \quad i_n d\omega = 0$$

3. **Mean Curvature Form**: Defined as:

   $$\mu := \mathcal{L}_n \chi$$

   where $$\chi$$ is the characteristic form of a bundle-like metric.

4. **Álvarez Class**: The cohomology class $$[\mu] \in H^1_b(F)$$ determines whether the flow is isometric.

## 7. Surface Gravity Analysis

For a degenerate horizon, we have the following result (Theorem 3.3):

$$\int_H \kappa\, d\tilde{g} = 0$$

where $$\tilde{g} = g_T + \alpha \otimes \alpha$$ is a Riemannian metric on $$H$$, and $$\alpha$$ is a 1-form such that $$\alpha(n) = 1$$.

For non-degenerate horizons, under the dominant energy condition, the flow is isometric, implying the existence of a Killing vector field tangent to the horizon.