---
layout: post
title: "Definition of topology and examples"
categories: lecture
---

A **topology** $$\tau$$ on a set $$X$$ is a collection of subsets of $$X$$ satisfying the following properties:

1. The sets $$X$$ and $$\emptyset$$ are in $$\tau$$
2. Given any collection $$(U_i)_{i \in I}$$ of sets in $$\tau$$, the union $$\bigcup_{i \in I} U_i$$ is in $$\tau$$
3. Given any two sets $$U$$ and $$V$$ in $$\tau$$, the intersection $$U \cap V$$ is in $$\tau$$.

We call sets in $$\tau$$ **open** or sometimes more precisely **$$\tau$$-open** when we are working with multiple topologies.

We defined <i>five</i> topologies living on the real line $$\mathbb{R}$$:

1. The standard (Euclidean) topology: open sets are arbitrary unions of open intervals $$(a, b)$$
2. Upper topology: open sets consist of intervals of the form $$(-\infty, a)$$
3. Lower limit topology: open sets are arbitrary unions of half-open intervals $$[a, b)$$
4. Discrete topology: *every* subset of the real line is open
5. Cofinite topology: a subset of the real line is open if and only if it is cofinite (i.e. its complement is finite)

When we have multiple topologies on the same space it makes sense to compare them.
Given two topologies $$\tau$$ and $$\tau'$$ on the same set $$X$$, we say that $$\tau$$ is **finer** than $$\tau'$$ if every set open in $$\tau'$$ is open in $$\tau$$ (think of this as saying that $$\tau$$ has <i>more</i> open sets).
In this case we also say that $$\tau'$$ is **coarser** than $$\tau$$.
On the other hand, if $$\tau$$ is neither finer nor coarser than $$\tau'$$ then we say that $$\tau$$ and $$\tau'$$ are **incomparable**.

### In-class exercises

1. Let $$\tau_1, ..., \tau_5$$ be the topologies on the real line listed above. Verify that they are indeed topologies.
    - We discovered that it's a bit difficult to show the lower limit topology is closed under finite intersections. A concept we will introduce next lecture will help.
    - A few students were not familiar with the notion of the supremum of a set of reals, which was necessary for showing the upper topology is closed under arbitarary unions. I will put a scaffolded exervice on the first written assignment covering this.
1. For each pair of topologies from $$\tau_1, ..., \tau_5$$, determine if one is finer or coarser than the other, or if they are incomparable.
    - We didn't finish going over this in class, so you will finish it on the first written assignment.

