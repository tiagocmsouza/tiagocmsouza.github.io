---
layout: post
title: "Optimization Theory - Introduction"
#date: 
description: An introductory and intuitive view of Optimization Theory
#img:  
---

The field of optimization can be unified by a few geometric principles of linear vector space theory (functional analysis in particular), which convey enough insight to solve complex infinite-dimensional problems.

Functional analysis should not be feared, however, as most of its main results are expressed as abstractions of intuitive geometric properties of finite-dimensional spaces. Once this intuition is build, it widens the range of problems that optimization theory can be applied. Indeed, the extension of these intuitive geometric insights to infinife-dimensional spaces is the reason why studing functional analysis becomes useful.

A first simple result is the Projection Theorem, which states that the perpendicular from a point to a hyperplane is the shortest line connecting the two of them. This same intuition has direct extensions to infinite-dimensional Hilbert spaces and forms the basis of least-squares estimation.

Extending the projection theorem to nonquadratic problems is possible to the Hahn-Banach theorem, which stands out as preserving the essence of the simple geometric ideas to more general vector spaces. That theorem has multiple versions, one of them being the existence of a separating hyperplane between a point and a convex set that does not contain it.

To express in terms of hyperplanes a problem originaly stated in terms of vectors in a space is the (one of the many) principle of duality. The geometric relation is established by reframing a minimization problem over vectors as a maximization problem over hyperplanes. For example, the shortest distance between a point and a convex set is equal to the maximum of the distances from the same point to a hyperplane separating it from the convex set.

Another optimization technique is the method of differential calculus, whose extension to infinite-dimesional spces is straightforward, and the geometric intuition remains the same, i.e., the tangent hyperplane at the optimal point is horizontal.

It becomes clear from the discussion above that convexity, hyperplanes and duality are essential parts of optimization theory. In fact, global optimization problems in linear spaces rely on convexity to reach its results, while differential conditions suffice for local theory.