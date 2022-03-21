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

Classical examples include \$l\_{p}\$, the sequence of real numbers \$\\{x\_{1}, x\_{2}, \dots\\}\$ for which \$\sum\_{i=1}^{\infty}{\|x\_{i}\|^p} < \infty\$ and \$0 \leq p \leq \infty\$. The norm is defined as \$\|\|x\|\|_{p} = \left( \sum\_{i=1}^{\infty}{\|x\_{i}\|^p} \right)^\frac{1}{p}\$ --- the space \$l\_{\infty}\$ is the space of bounded sequences with the norm defined as \$\|\| x \|\|\_{\infty} = \sup\_{i}{\|x\_{i}\|}\$. 

\$L\_{p}[a,b]\$ spaces, for \$1 \leq p \leq \infty \$, consists of real-valued measurable functions on \$[a,b]\$ for which \$\|x(t)\|^{p}\$ is Lebesgue intergrable and the norm is defined as \$\|\|x\|\|\_{p} = \left( \int\_{a}^{b}{\|x(t)\|^{p} \\, dt} \right)^\frac{1}{p}\$ --- when \$0 < p < 1\$ these are metric spaces, whose metric is not induced by a norm. Note that \$\|\|x\|\|\_{p} = 0\$ on this space does not necessarily imply that \$x\$ is the zero vector, as it may be different from zero in a set of measure zero. However, \$L\_{p}[a,b]\$ is a normed linear space if no distinction is made between function equal almost everywhere.

The space \$L\_{\infty}[a,b]\$ is analogous to \$l\_{\infty}\$, defined as the space of all bounded Lebesgue measurable functions on \$[a,b]\$, excepet for a set of measure zero. Since we regard as equivalent two functions differing only on a set of measure zero, defining the norm as \$\sup\_{a \leq t \leq b}{\|x(t)\|}\$ is ambiguous, as this supremum is different for different functions equivalent to \$x\$. Therefore, the norm is defined as \$\|\|x\|\|\_{\infty} = \text{ess} \sup \|x(t)\| \$ (essential supremum) \$\equiv \inf\_{y(t) = x(t) a.e.}{[\sup \|y(t)\|]}\$.

Transformations are objects that make the study of linear spaces interesting and useful, but do not forget the need of a topology, usually induced by a norm in vectoral spaces, to define a notion of continuity (which depends on the topological structure on both spaces that the transformation is defined on).

A key concept of analysis is convergence, usually to prove the existence of a vector satisfying some desired property. To do so, it is common to define a sequence of vectors converging to a limit and, in many cases, this limit can be shown to satisfy that desired property. Spaces of particular interest are those in which every Cauchy sequence has a limit, known as complete spaces --- a complete normed space is a Banach space. Having this property allows the identification of convergence sequences without identifying their limits. Because of that, in applied problems, it is intersting to formulate it in terms of Banach space rather than in other (maybe incomplete) spaces: the reason for that is that the desired optimal vector is the limit of a sequence and the Cauchy criterion for convergence is a test for convergence, which can be applied when the limit is unknown, provided the the underlying space is complete.

The vector space of continuous functions with the norm \$ \|\|x\|\| = \int\_{0}^{1}{\|x(t)\| \, dt} \$ is not complete, as there are Cauchy sequences that converge to non-continuous functions. However \$C[0,1]\$, the space of continuous functions with the norm \$ \|\|x\|\| = \max\_{0 \leq t \leq 1}{\|x(t)\|} \$, is complete. Other examples of Banach spaces are \$l\_{p}\$ and \$L\_{p}\$, with \$1 \leq p \leq \infty\$.