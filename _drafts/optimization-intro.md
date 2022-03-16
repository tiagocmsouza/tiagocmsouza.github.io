---
layout: post
title: "Optimization Theory - Introduction"
#date: 
description: An introductory and intuitive view of Optimization Theory
#img:  
---

The field of optimization can be unified by a few geometric principles of linear vector space theory, which convey enough insight to solve complex problems. Indeed, the extension of these intuitive geometric insights to infinife-dimensional spaces is the reason why studing functional analysis becomes useful. Functional analysis should not be feared, however, as most of its main results are expressed as abstractions of intuitive geometric properties of finite-dimensional spaces. Once this intuition is build, it widens the range of problems that optimization theory can be applied to. 

A first simple result is the Projection Theorem, which states that the perpendicular from a point to a hyperplane is the shortest line connecting the two of them. This same intuition has direct extensions to infinite-dimensional Hilbert spaces and forms the basis of least-squares estimation. Extending the projection theorem to nonquadratic problems is possible due to the Hahn-Banach theorem, which stands out as preserving the essence of simple geometric ideas to more general vector spaces (even without a topology defined over it). That theorem has multiple versions, one of them being the existence of a separating hyperplane between convex sets.

To express a problem in terms of hyperplanes that was originaly stated in terms of vectors in a space is the (one of the many) principles of duality. The geometric relation is established by reframing a minimization problem over vectors as a maximization problem over hyperplanes. For example, the shortest distance between a point and a convex set is equal to the maximum of the distances from the same point to a hyperplane separating it from the convex set.

Another optimization technique is the method of differential calculus, whose extension to infinite-dimesional spces is straightforward, and the geometric intuition remains the same, i.e., the tangent hyperplane at the optimal point is horizontal.

It should be stressed that convexity, hyperplanes and duality are essential parts of optimization theory. In fact, global optimization problems in linear spaces rely on convexity to reach its results, while differential conditions suffice for local theory.

The introduction of topological properties (be it by defining a metric, a norm or an inner product), such as convergence and open and closed sets, is what distinghuishes functional analysis from linear algebra. However, optimization theory can be proven in purely algebric terms, prescinding from a topology.

Convexity and Cones are seen as generalizations of the concepts of subspaces and linear varieties, since both of these are convex cones. In fact, convexity is deemed as the fundamental algebraic concept of vector spaces. Note, however, convex cones also arise when defining positive vectors in a vector space.

The axioms of vector spaces describe algebraic properties only (such as addition, scalar multiplication and linear combinations), which makes the introduction of a measure of distance necessary to explore topological concepts like opennes, closure, convergence and completeness. In vectoral spaces this is usually done by introducing a norm, an abstraction of the concept of length. Moreover, it can be shown that interior and taking closure preserves convexity, subspaces, linear varieties and cones.

Classical examples include $l_{p}$, the sequence of real numbers $\\{x_{1}, x_{2}, \dots\\}$ for which $\sum_{i=1}^{\infty}{\|x_{i}\|^p} < \infty$ and the norm is defined as $\|\|x\|\|_{p} = \left( \sum_{i=1} \right)^\frac{1}{p}$.

A key concept of analysis is convergence, usually to prove the existence of a vector satisfying some desired property. To do so, it is common to define a sequence of vectors converging to a limit and, in many cases, this limit can be shown to satisfy that desired property.

Transformations are objects that make the study of linear spaces interesting and useful, but do not forget the need of a topology, usually induced by a norm in vectoral spaces, to define a notion of continuity (which depends on the topological structure on both spaces that the transformation is defined on).